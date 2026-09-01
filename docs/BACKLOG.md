# Backlog del Proyecto: Sistema para el Control y Comercialización de la Producción de Miel

**Organización:** Unión de Productores de Miel de San Juan Ñumí, Oaxaca  
**Materia:** Gestión de Proyectos de Software  
**Fuente de historias de usuario base:** `problematicas/problematica-1.md`

---

## Estructura del Backlog por Fases

El desarrollo del sistema se organiza en tres fases evolutivas para garantizar entregas de valor continuo y alinearse con hitos de evaluación técnica y financiera.

---

### Fase 1 – Producto Mínimo Viable (MVP)
* **Objetivo:** Digitalizar la operación básica de captura en campo, registro de colmenas y control de inventario de miel en bodega.
* **Historias de Usuario Existentes Incorporadas:**
  * **HU-01: Registro de productores y colmenas:** Como administrador de la unión, quiero registrar a los productores locales y la ubicación/cantidad de sus colmenas para tener un padrón confiable.
  * **HU-02: Registro de producción por cosecha:** Como apicultor/administrador, quiero registrar los kilogramos de miel cosechados por temporada y tipo de floración para llevar el control de extracción.
  * **HU-03: Control de inventario en bodega:** Como encargado de almacén, quiero registrar las entradas, salidas y existencias de cubetas/tambores de miel para evitar pérdidas y descadres.

---

### Fase 2 – Integración y Pruebas
* **Objetivo:** Incorporar la comercialización local, registro de clientes y la generación de reportes operativos de la organización.
* **Historias de Usuario Existentes Incorporadas:**
  * **HU-04: Registro de ventas y clientes:** Como encargado de comercialización, quiero registrar las ventas realizadas, montos y datos del cliente para dar seguimiento a la comercialización.
  * **HU-05: Reporte mensual de producción y ventas:** Como directivo de la unión, quiero generar reportes consolidados mensuales para evaluar la productividad y tomar decisiones financieras.

---

### Fase 3 – Operación, Expansión e Infraestructura Futura
* **Objetivo:** Asegurar la sostenibilidad del sistema, monitoreo continuo y evaluar la viabilidad de adopción de infraestructura Web3/on-chain.
* **Aviso de Alcance:** *Las siguientes entradas representan actividades futuras de ingeniería, infraestructura y mantenimiento técnico. No corresponden a las historias de usuario de negocio preexistentes.*

* **Actividades Futuras:**
  * **AF-01: Despliegue en producción:** Configuración del servidor Web/Cloud e infraestructura de base de datos segura para acceso remoto desde San Juan Ñumí.
  * **AF-02: Implementación de seguridad y control de acceso:** Configuración de roles, autenticación robusta y encriptación de datos sensibles.
  * **AF-03: Monitoreo y observabilidad:** Configuración de métricas de disponibilidad del sistema y registro de logs de eventos.
  * **AF-04: Mantenimiento correctivo y evolutivo:** Soporte técnico post-despliegue y resolución de incidentes en producción.
  * **AF-05: Evaluación de integración con Stellar:** Análisis técnico para el posible uso de la red Stellar en pagos transfronterizos o emisión de activos digitales representativos de la producción de miel.
  * **AF-06: Evaluación de integración con Drips Protocol:** Análisis de viabilidad para recibir transferencias continuas o donaciones en flujo (streaming) para el sostenimiento del software de código abierto.

---

## Matriz de Trazabilidad con Financiamiento

| Fase | Alcance Técnico | Vinculación a Tramo de Financiamiento |
| :--- | :--- | :--- |
| **Fase 1 (MVP)** | HU-01, HU-02, HU-03 | **Tranche 1 (SCF Build Award):** Financia el desarrollo inicial del núcleo funcional del sistema y la base de datos de productores. |
| **Fase 2 (Integración y Pruebas)** | HU-04, HU-05 | **Tranche 2 (SCF Build Award / Testnet):** Financia la consolidación de módulos comerciales, pruebas de integración y elaboración del modelo de amenazas. |
| **Fase 3 (Operación y Expansión)** | AF-01 a AF-06 | **Tranche 3 (SCF Mainnet / Drips Protocol):** Financia el despliegue en producción, mantenimiento a largo plazo y la evaluación de flujos continuos de fondos. |

