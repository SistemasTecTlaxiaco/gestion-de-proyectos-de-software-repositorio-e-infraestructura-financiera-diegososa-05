# Investigación de Infraestructura Financiera y Estrategia de Financiamiento

**Proyecto:** Sistema para el Control y Comercialización de la Producción de Miel  
**Organización:** Unión de Productores de Miel de San Juan Ñumí, Oaxaca  
**Materia:** Gestión de Proyectos de Software  
**Fecha de consulta de fuentes:** 31 de agosto de 2026  

---

## 1. Requisitos de Stellar Community Fund (SCF)

El **Stellar Community Fund (SCF)** es un programa de subvenciones de la *Stellar Development Foundation (SDF)* diseñado para respaldar a desarrolladores y empresas que construyen aplicaciones y herramientas sobre la red de bloques Stellar.

### 1.1 Requisitos Vigentes de Postulación (Build Award)
De acuerdo con la documentación oficial del SCF Handbook, para postular una iniciativa en la modalidad *Build Award*, los proyectos deben cumplir con las siguientes condiciones:
1. **Alineación Técnica:** La propuesta debe integrar la red Stellar o contratos inteligentes Soroban como componente central del sistema (p. ej., gestión de pagos, tokenización de activos o registro de trazabilidad).
2. **Prueba de Ajuste Producto-Mercado (Product-Market Fit):** Demostrar tracción real de usuarios o una necesidad de mercado claramente validada por un equipo con experiencia en el dominio del problema.
3. **Estructura Técnica Detallada:** Presentar una arquitectura de sistema completa, plan de trabajo sin ambigüedades y una justificación clara de costos basada exclusivamente en desarrollo técnico.
4. **Esquema de Tranches (3 Entregables):** La solicitud presupuestal debe dividirse en tres etapas obligatorias:
   * **Tranche 1 (MVP):** Desarrollo de la primera versión funcional.
   * **Tranche 2 (Testnet):** Pruebas en red de prueba, incluyendo un **Modelo de Amenazas (Threat Model)** y un **Plan de Monitoreo On-Chain**.
   * **Tranche 3 (Mainnet Launch):** Despliegue en red principal con compromiso de métricas medibles de uso (volumen de transacciones, cuentas activas o valor registrado).
5. **Cumplimiento Legal y KYC:** Superar la verificación de identidad (KYC/KYB) y controles de sanciones internacionales coordinados por la SDF.

### 1.2 Criterios de Evaluación
Las propuestas son evaluadas por un panel de la comunidad Stellar mediante los siguientes criterios:
* **Impacto y Utilidad:** ¿El proyecto resuelve un problema del mundo real y aporta valor medible al ecosistema?
* **Factibilidad Técnica y Capacidad del Equipo:** ¿La arquitectura planteada es sólida y el equipo posee la capacidad técnica para ejecutarla?
* **Presupuesto Razonable:** El presupuesto solicitado (denominado en USD y liquidado en XLM) debe ser proporcional al alcance y alinearse con las guías financieras del SCF.
* **Diferenciación:** Grado de innovación o adaptación adecuada de la tecnología a un sector específico.

* **Fuente oficial:** [Stellar Community Fund Handbook - Submission Criteria](https://stellar.gitbook.io/scf-handbook/scf-awards/build-award/submission-criteria)  
* **Fecha de consulta:** 31 de agosto de 2026

---

## 2. Funcionamiento de Drips Protocol

### 2.1 Definición y Streaming de Fondos On-Chain
**Drips Protocol** es un protocolo descentralizado, autónomo y no custodial construido sobre la red Ethereum (y redes EVM compatibles). Permite realizar **streaming de fondos on-chain**, lo cual consiste en la transferencia continua de tokens ERC-20 calculada segundo a segundo a través de contratos inteligentes. 

A diferencia de las transferencias bancarias tradicionales o los pagos por bloques fijos, el streaming permite que el emisor configure una tasa de flujo de dinero (ej. $X$ tokens por segundo). El receptor acumula dicho flujo en tiempo real en la cadena de bloques y puede retirar (*claim*) los fondos acumulados en el momento que lo desee.

### 2.2 Requisitos para Recibir Fondos
Para que el proyecto de la Unión de Productores de Miel pueda recibir streaming o donaciones a través de Drips Protocol se requiere:
1. **Identidad Web3 o Configuración de Repositorio:** Una dirección de billetera (*wallet*) compatible con Ethereum (EVM) controlada por la organización. Alternativamente, Drips permite vincular repositorios públicos de GitHub mediante un archivo de configuración `FUNDING.json` ubicado en la rama predeterminada, validado por un oráculo Chainlink.
2. **Listas de Licencias/Dependencias (Drip Lists):** Configurar la división de ingresos (*dependency splitting*), lo cual permite que un porcentaje de las donaciones recibidas se reenvíe automáticamente a proyectos de código abierto de los cuales dependa el software.

### 2.3 Costos, Límites y Consideraciones
* **Costos de Transacción (Gas Fees):** La creación de un flujo (*stream*), el retiro de fondos (*claim*) y la actualización de listas requieren ejecutar transacciones en la red Ethereum, lo que implica el pago de tarifas de red (*gas*).
* **Custodia de Llaves Privadas:** Al ser un protocolo no custodial, la pérdida de las llaves privadas de la billetera receptora resulta en la pérdida irreversible de los fondos acumulados.
* **Volatilidad de Activos:** Los fondos recibidos mediante tokens ERC-20 sufren la fluctuación de precio del mercado cripto si no se utilizan criptomonedas estables (*pegged* como USDC o DAI).

* **Fuente oficial:** [Drips Network Documentation](https://docs.drips.network/the-protocol/overview/)  
* **Fecha de consulta:** 31 de agosto de 2026

---

## 3. Relación entre el Backlog y los Tramos de Financiamiento

La estrategia de financiamiento del proyecto no contempla recibir ingresos de forma inmediata, sino alinear el avance del código con posibles fondos externos:

1. **Fase 1 (MVP) ── Vinculada a SCF Tranche 1:**
   * *Qué se financiaría:* Horas de desarrollo para completar las historias `HU-01`, `HU-02` y `HU-03` (módulos de productores, cosechas e inventario de miel).
   * *Por qué:* Es la etapa mínima requerida para demostrar un software funcional de captura de datos antes de solicitar integraciones complejas.

2. **Fase 2 (Integración y Pruebas) ── Vinculada a SCF Tranche 2:**
   * *Qué se financiaría:* Implementación de `HU-04` y `HU-05` (comercialización y reportes) junto con el diseño del modelo de seguridad y pruebas en Testnet.
   * *Por qué:* Permite validar la estabilidad del sistema y cumplir con los requisitos de seguridad que exige Stellar para pasar a redes de producción.

3. **Fase 3 (Operación y Expansión) ── Vinculada a SCF Tranche 3 y Drips Protocol:**
   * *Qué se financiaría:* Despliegue en Mainnet (`AF-01`), mantenimiento continuo (`AF-04`), y la evaluación técnica para habilitar streaming de aportaciones comunitarias a través de Drips (`AF-06`).
   * *Por qué:* Garantiza la sostenibilidad operativa del software en San Juan Ñumí a largo plazo mediante infraestructura descentralizada.

---

## 4. El Hueco Honesto (Requisitos Pendientes)

Para presentar una postulación real a fuentes de financiamiento *on-chain*, el proyecto reconoce de manera transparente que **aún no cumple** con los siguientes requisitos:

| Requisito Faltante | Estado Actual | Plan de Acción para Solucionarlo | Fecha Estimada de Cierre |
| :--- | :--- | :--- | :--- |
| **1. Integración con Soroban / Stellar SDK** | El código actual es un prototipo local sin conexión a redes blockchain. | Desarrollar el módulo de conexión mediante `stellar-sdk` en la Fase 3 de evaluación. | 15 de noviembre de 2026 |
| **2. Modelo de Amenazas y Plan de Monitoreo** | No se ha redactado la documentación de análisis de riesgos informáticos. | Elaborar la plantilla de *Threat Modeling* exigida por SCF durante la Fase 2. | 15 de octubre de 2026 |
| **3. Billetera de la Organización y `FUNDING.json`** | La Unión de Productores no posee wallet EVM ni archivo `FUNDING.json` en GitHub. | Crear la billetera multisig institucional y configurar el archivo de soporte en el repositorio. | 30 de septiembre de 2026 |
| **4. Despliegue en Testnet y Métrica de Uso** | El sistema no está desplegado en ningún servidor accesible públicamente. | Configurar el entorno de pruebas en la nube para medir el uso real por parte de los apicultores. | 30 de octubre de 2026 |

---

## 5. Bibliografía

1. **Stellar Development Foundation.** (2026). *Stellar Community Fund Handbook: Build Award Submission Criteria*. Recuperado de: https://stellar.gitbook.io/scf-handbook/scf-awards/build-award/submission-criteria [Fuente primaria en inglés]
2. **Drips Protocol Team.** (2026). *Drips Technical Overview & Protocol Specification*. Recuperado de: https://docs.drips.network/the-protocol/overview/ [Fuente primaria en inglés]
3. **Drips Network.** (2026). *Drips Application Repository and GitHub Integration Specs*. GitHub. Recuperado de: https://github.com/drips-network/app [Fuente primaria en inglés]
