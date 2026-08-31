# Financiamiento del Proyecto

## Gestión de Proyectos de Software

**Materia:** Gestión de Proyectos de Software (SCG-1009)  
**Institución:** TECNM Campus Tlaxiaco  
**Periodo:** Agosto – Diciembre 2026  

---

## 1. Introducción

El financiamiento es un elemento importante dentro de la gestión de proyectos de software, debido a que permite planificar los recursos necesarios para realizar actividades de desarrollo, pruebas, infraestructura, seguridad, integración y puesta en producción.

En este documento se investigan dos elementos relacionados con la infraestructura financiera de proyectos tecnológicos: el **Stellar Community Fund (SCF)** y el **protocolo Drips**.

El Stellar Community Fund es un programa de financiamiento del ecosistema Stellar que busca apoyar proyectos que desarrollan soluciones utilizando la tecnología de Stellar y Soroban.

Por otra parte, Drips es un protocolo orientado a la distribución continua de fondos mediante tecnología blockchain, principalmente dentro del ecosistema Ethereum y redes compatibles con EVM.

El propósito de esta investigación no es realizar transacciones reales ni desplegar fondos on-chain. La finalidad es conocer los requisitos reales de estos mecanismos, analizar sus características y relacionarlos con el backlog del proyecto organizado por fases.

---

# 2. Stellar Community Fund (SCF)

## 2.1 ¿Qué es el Stellar Community Fund?

El **Stellar Community Fund (SCF)** es un programa del ecosistema Stellar que proporciona financiamiento a proyectos que desarrollan soluciones utilizando la red Stellar.

El programa busca apoyar diferentes tipos de proyectos y propuestas que puedan aportar valor al ecosistema.

Para esta práctica se toma como referencia principalmente el **Build Award**, debido a que contempla el desarrollo de proyectos mediante diferentes etapas.

---

## 2.2 Requisitos y criterios de evaluación

De acuerdo con la información oficial del Stellar Community Fund, los proyectos deben presentar una propuesta que permita evaluar diferentes aspectos del proyecto.

Entre los principales criterios se encuentran:

- **Product Market Fit:** relación entre el producto y las necesidades de los usuarios.
- **Submission Quality:** calidad y claridad de la propuesta presentada.
- **Use of Stellar:** utilización de la tecnología y herramientas del ecosistema Stellar.
- **Integration Plan:** planificación de la integración con Stellar.
- **Ready to Build:** grado de preparación del equipo para comenzar o continuar el desarrollo.
- **Budget & Tranches:** presupuesto y distribución del financiamiento mediante diferentes tramos.

Estos criterios permiten determinar si un proyecto presenta una propuesta viable y si existe una justificación adecuada para proporcionar financiamiento.

---

## 2.3 Tramos del financiamiento

El Build Award del Stellar Community Fund organiza el desarrollo mediante diferentes etapas o tramos.

La estructura publicada actualmente contempla:

| Tramo | Etapa | Propósito |
|---|---|---|
| Tranche #1 | MVP | Desarrollo del producto mínimo viable |
| Tranche #2 | Testnet | Pruebas y validación técnica |
| Tranche #3 | Mainnet | Implementación en la red principal |

Esta estructura permite relacionar el financiamiento con resultados concretos del desarrollo.

Es importante aclarar que esta estructura se utiliza en este documento como referencia para organizar nuestro proyecto. **El equipo no cuenta actualmente con un financiamiento aprobado por el Stellar Community Fund.**

---

## 2.4 Relación con nuestro proyecto

Los requisitos del SCF permiten identificar varios aspectos que nuestro proyecto debe considerar antes de realizar una posible postulación.

Entre ellos se encuentran:

1. Definir claramente el problema que se pretende solucionar.
2. Identificar a los usuarios objetivo.
3. Contar con un producto o prototipo funcional.
4. Demostrar el avance del proyecto.
5. Justificar el uso de Stellar.
6. Definir un plan de integración.
7. Elaborar un presupuesto.
8. Organizar el desarrollo mediante fases.
9. Establecer resultados verificables para cada etapa.

Por lo tanto, el backlog del proyecto puede organizarse de manera que cada fase produzca resultados que posteriormente puedan ser utilizados como evidencia de avance.

---

## 2.5 Fuente oficial y fecha de consulta

**Fuente oficial:** Stellar Community Fund – Build Awards

https://communityfund.stellar.org/awards

**Fecha de consulta:** 31 de agosto de 2026.

---

# 3. Drips Protocol

## 3.1 ¿Qué es Drips?

**Drips** es un protocolo que permite distribuir fondos de manera continua mediante tecnología blockchain.

Su funcionamiento está relacionado principalmente con Ethereum y redes compatibles con EVM.

Una de sus características principales es el uso de **streams**, mediante los cuales los fondos pueden distribuirse progresivamente hacia uno o varios receptores.

---

## 3.2 ¿Qué es el streaming de fondos?

El streaming de fondos consiste en distribuir una cantidad de recursos de manera continua durante un periodo determinado.

A diferencia de una transferencia tradicional, en la que una cantidad se envía de una sola vez, un stream utiliza una tasa de distribución.

Por ejemplo, conceptualmente se puede establecer una cantidad que se distribuye progresivamente a un receptor con una determinada tasa por segundo.

El protocolo registra esta información mediante contratos inteligentes y permite que los receptores recopilen posteriormente los fondos que les corresponden.

---

## 3.3 ¿Qué se necesita para recibir fondos?

Para recibir fondos mediante Drips es necesario contar con una cuenta o dirección compatible con las redes soportadas por el protocolo.

El receptor puede acumular fondos de acuerdo con los streams configurados.

Posteriormente, los fondos disponibles pueden ser recopilados mediante las operaciones correspondientes del protocolo.

Estas operaciones se realizan mediante tecnología blockchain y pueden implicar costos de gas.

---

## 3.4 Límites y consideraciones

El uso de Drips implica considerar diferentes aspectos técnicos:

- El protocolo utiliza redes compatibles con EVM.
- Las operaciones se realizan mediante contratos inteligentes.
- Los streams utilizan una tasa de distribución.
- Los fondos se acumulan para los receptores.
- Los receptores deben recopilar los fondos disponibles.
- Las operaciones pueden generar costos de gas.
- Existen límites relacionados con la cantidad de receptores y la configuración de los streams.

La documentación técnica de Drips indica que una configuración de streams puede manejar hasta **100 receptores**.

Por lo tanto, antes de utilizar este mecanismo es necesario analizar los costos, las redes disponibles y la configuración requerida.

---

## 3.5 Relación con nuestro proyecto

Drips puede considerarse como una alternativa tecnológica para distribuir recursos de manera continua.

Sin embargo, su utilización dependería de las características y necesidades específicas de nuestro proyecto.

Además, es importante distinguir ambas tecnologías:

- El **Stellar Community Fund** corresponde a un mecanismo de financiamiento del ecosistema Stellar.
- **Drips** corresponde a un protocolo de distribución continua de fondos basado principalmente en Ethereum y redes EVM.

Por lo tanto, Drips no debe considerarse como un componente propio del Stellar Community Fund.

---

## 3.6 Fuente técnica

**Documentación oficial de Drips:**

https://docs.drips.network/

**Documentación técnica:**

https://docs.drips.network/the-protocol/advanced/drips-inner-workings/

**Fecha de consulta:** 31 de agosto de 2026.

---

# 4. Backlog por fases y financiamiento

El backlog del proyecto se relaciona con las etapas de desarrollo utilizadas como referencia por el Stellar Community Fund.

La finalidad es identificar qué actividades podrían asociarse hipotéticamente con cada tramo de financiamiento.

---

## 4.1 Fase 1 – MVP

### Objetivo

Construir una primera versión funcional del proyecto que permita validar la propuesta principal.

### Actividades

- Definición de requisitos.
- Diseño inicial.
- Desarrollo de funcionalidades principales.
- Implementación del prototipo.
- Pruebas iniciales.
- Validación con usuarios.

### Relación con financiamiento

Esta fase se relacionaría hipotéticamente con:

**Tranche #1 – MVP**

Los recursos podrían utilizarse para cubrir actividades relacionadas con el desarrollo inicial y validación del producto.

---

## 4.2 Fase 2 – Testnet / Validación

### Objetivo

Validar técnicamente la solución antes de una implementación definitiva.

### Actividades

- Integración de componentes.
- Pruebas funcionales.
- Pruebas de seguridad.
- Corrección de errores.
- Validación técnica.
- Integración con Stellar, en caso de que corresponda al proyecto.

### Relación con financiamiento

Esta fase se relacionaría hipotéticamente con:

**Tranche #2 – Testnet**

El financiamiento permitiría continuar con el desarrollo y realizar pruebas que demuestren el funcionamiento técnico de la solución.

---

## 4.3 Fase 3 – Mainnet / Implementación

### Objetivo

Preparar una versión estable para usuarios reales.

### Actividades

- Implementación de la versión final.
- Mejoras de rendimiento.
- Seguridad.
- Documentación.
- Monitoreo.
- Soporte inicial.

### Relación con financiamiento

Esta fase se relacionaría hipotéticamente con:

**Tranche #3 – Mainnet**

Los recursos permitirían realizar las actividades necesarias para pasar de una versión validada a una implementación estable.

---

## 4.4 Tabla de relación

| Fase del proyecto | Resultado esperado | Posible tramo |
|---|---|---|
| Fase 1 | MVP funcional | Tranche #1 |
| Fase 2 | Testnet / validación | Tranche #2 |
| Fase 3 | Mainnet / implementación | Tranche #3 |

Esta relación representa una planificación hipotética del equipo y no implica que el proyecto tenga financiamiento aprobado.

---

# 5. El hueco honesto

Investigar los requisitos del Stellar Community Fund y de Drips no significa que nuestro proyecto cumpla actualmente con todos los requisitos necesarios para recibir financiamiento.

Por esta razón, se identifican los siguientes aspectos pendientes.

| Requisito pendiente | Acción para cerrarlo | Fecha estimada |
|---|---|---|
| Validación con usuarios | Realizar pruebas y recopilar retroalimentación | Septiembre 2026 |
| Integración con Stellar | Definir y validar los componentes necesarios | Octubre 2026 |
| Presupuesto | Elaborar un presupuesto detallado por fase | Octubre 2026 |
| Evidencia técnica | Completar pruebas y documentación | Noviembre 2026 |
| Preparación para una posible postulación | Revisar nuevamente los requisitos oficiales | Noviembre 2026 |

Actualmente, el proyecto **NO se considera listo para realizar una postulación real**.

El objetivo es utilizar estos pendientes como guía para continuar mejorando el proyecto.

Las fechas son estimaciones académicas del equipo y pueden modificarse de acuerdo con el avance del proyecto.

---

# 6. Organización del repositorio

La documentación relacionada con la actividad se organiza de la siguiente manera:

```text
/
├── README.md
├── FINANCIAMIENTO.md
├── LICENSE
│
├── docs/
│   └── BACKLOG.md
│
└── demás archivos del proyecto
---

# 2. Stellar Community Fund (SCF)

## 2.1 ¿Qué es el Stellar Community Fund?

El **Stellar Community Fund (SCF)** es un programa del ecosistema Stellar que proporciona financiamiento a proyectos que desarrollan soluciones utilizando la red Stellar.

El programa busca apoyar diferentes tipos de proyectos y propuestas que puedan aportar valor al ecosistema.

Para esta práctica se toma como referencia principalmente el **Build Award**, debido a que contempla el desarrollo de proyectos mediante diferentes etapas.

---

## 2.2 Requisitos y criterios de evaluación

De acuerdo con la información oficial del Stellar Community Fund, los proyectos deben presentar una propuesta que permita evaluar diferentes aspectos del proyecto.

Entre los principales criterios se encuentran:

- **Product Market Fit:** relación entre el producto y las necesidades de los usuarios.
- **Submission Quality:** calidad y claridad de la propuesta presentada.
- **Use of Stellar:** utilización de la tecnología y herramientas del ecosistema Stellar.
- **Integration Plan:** planificación de la integración con Stellar.
- **Ready to Build:** grado de preparación del equipo para comenzar o continuar el desarrollo.
- **Budget & Tranches:** presupuesto y distribución del financiamiento mediante diferentes tramos.

Estos criterios permiten determinar si un proyecto presenta una propuesta viable y si existe una justificación adecuada para proporcionar financiamiento.

---

## 2.3 Tramos del financiamiento

El Build Award del Stellar Community Fund organiza el desarrollo mediante diferentes etapas o tramos.

La estructura publicada actualmente contempla:

| Tramo | Etapa | Propósito |
|---|---|---|
| Tranche #1 | MVP | Desarrollo del producto mínimo viable |
| Tranche #2 | Testnet | Pruebas y validación técnica |
| Tranche #3 | Mainnet | Implementación en la red principal |

Esta estructura permite relacionar el financiamiento con resultados concretos del desarrollo.

Es importante aclarar que esta estructura se utiliza en este documento como referencia para organizar nuestro proyecto. **El equipo no cuenta actualmente con un financiamiento aprobado por el Stellar Community Fund.**

---

## 2.4 Relación con nuestro proyecto

Los requisitos del SCF permiten identificar varios aspectos que nuestro proyecto debe considerar antes de realizar una posible postulación.

Entre ellos se encuentran:

1. Definir claramente el problema que se pretende solucionar.
2. Identificar a los usuarios objetivo.
3. Contar con un producto o prototipo funcional.
4. Demostrar el avance del proyecto.
5. Justificar el uso de Stellar.
6. Definir un plan de integración.
7. Elaborar un presupuesto.
8. Organizar el desarrollo mediante fases.
9. Establecer resultados verificables para cada etapa.

Por lo tanto, el backlog del proyecto puede organizarse de manera que cada fase produzca resultados que posteriormente puedan ser utilizados como evidencia de avance.

---

## 2.5 Fuente oficial y fecha de consulta

**Fuente oficial:** Stellar Community Fund – Build Awards

https://communityfund.stellar.org/awards

**Fecha de consulta:** 31 de agosto de 2026.
---

# 3. Drips Protocol

## 3.1 ¿Qué es Drips?

**Drips** es un protocolo que permite distribuir fondos de manera continua mediante tecnología blockchain.

Su funcionamiento está relacionado principalmente con Ethereum y redes compatibles con EVM.

Una de sus características principales es el uso de **streams**, mediante los cuales los fondos pueden distribuirse progresivamente hacia uno o varios receptores.

---

## 3.2 ¿Qué es el streaming de fondos?

El streaming de fondos consiste en distribuir una cantidad de recursos de manera continua durante un periodo determinado.

A diferencia de una transferencia tradicional, en la que una cantidad se envía de una sola vez, un stream utiliza una tasa de distribución.

Por ejemplo, conceptualmente se puede establecer una cantidad que se distribuye progresivamente a un receptor con una determinada tasa por segundo.

El protocolo registra esta información mediante contratos inteligentes y permite que los receptores recopilen posteriormente los fondos que les corresponden.

---

## 3.3 ¿Qué se necesita para recibir fondos?

Para recibir fondos mediante Drips es necesario contar con una cuenta o dirección compatible con las redes soportadas por el protocolo.

El receptor puede acumular fondos de acuerdo con los streams configurados.

Posteriormente, los fondos disponibles pueden ser recopilados mediante las operaciones correspondientes del protocolo.

Estas operaciones se realizan mediante tecnología blockchain y pueden implicar costos de gas.

---

## 3.4 Límites y consideraciones

El uso de Drips implica considerar diferentes aspectos técnicos:

- El protocolo utiliza redes compatibles con EVM.
- Las operaciones se realizan mediante contratos inteligentes.
- Los streams utilizan una tasa de distribución.
- Los fondos se acumulan para los receptores.
- Los receptores deben recopilar los fondos disponibles.
- Las operaciones pueden generar costos de gas.
- Existen límites relacionados con la cantidad de receptores y la configuración de los streams.

La documentación técnica de Drips indica que una configuración de streams puede manejar hasta **100 receptores**.

Por lo tanto, antes de utilizar este mecanismo es necesario analizar los costos, las redes disponibles y la configuración requerida.

---

## 3.5 Relación con nuestro proyecto

Drips puede considerarse como una alternativa tecnológica para distribuir recursos de manera continua.

Sin embargo, su utilización dependería de las características y necesidades específicas de nuestro proyecto.

Además, es importante distinguir ambas tecnologías:

- El **Stellar Community Fund** corresponde a un mecanismo de financiamiento del ecosistema Stellar.
- **Drips** corresponde a un protocolo de distribución continua de fondos basado principalmente en Ethereum y redes EVM.

Por lo tanto, Drips no debe considerarse como un componente propio del Stellar Community Fund.

---

## 3.6 Fuente técnica

**Documentación oficial de Drips:**

https://docs.drips.network/

**Documentación técnica:**

https://docs.drips.network/the-protocol/advanced/drips-inner-workings/

**Fecha de consulta:** 31 de agosto de 2026.
