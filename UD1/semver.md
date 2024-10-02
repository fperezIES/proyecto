# Versionado Semántico

El versionado de software es una parte crítica en el ciclo de vida del desarrollo de proyectos. Es fundamental para gestionar cambios, comunicarse con equipos y usuarios, y asegurar la interoperabilidad entre sistemas y dependencias. En el desarrollo ágil, donde los cambios son frecuentes y las entregas son rápidas, utilizar un sistema de versionado coherente y claro es esencial.

## ¿Qué es el Versionado Semántico?

El **versionado semántico** es una convención que sigue un esquema de tres números separados por puntos, en el formato `MAJOR.MINOR.PATCH`. Fue propuesto por Tom Preston-Werner (cofundador de GitHub) en 2013, con el objetivo de crear un sistema de numeración que refleje la evolución del software y su compatibilidad con versiones anteriores.

La notación se interpreta de la siguiente manera:

- **MAJOR** (versión mayor): Se incrementa cuando se realizan cambios incompatibles con versiones anteriores. Por ejemplo, cambios en la API que requieren que los sistemas dependientes modifiquen su código.
- **MINOR** (versión menor): Se incrementa cuando se añaden nuevas funcionalidades que son compatibles con versiones anteriores. Los usuarios pueden actualizar sin necesidad de hacer cambios adicionales.
- **PATCH** (parche o corrección): Se incrementa cuando se hacen correcciones de errores o mejoras menores que no afectan la compatibilidad ni añaden nuevas funcionalidades.

**Ejemplo:** La versión **2.3.4** indica:

- **2**: Segunda versión mayor (posiblemente con cambios importantes respecto a la versión 1.x.x).
- **3**: Tercera actualización de nuevas funcionalidades en esta versión mayor.
- **4**: Cuarta corrección de errores o ajustes menores dentro de la versión 2.3.

## Reglas del Versionado Semántico

1. **Incremento de MAJOR (Cambios incompatibles):** Si realizas cambios que rompen la compatibilidad con versiones anteriores, incrementa el número mayor.
   - *Ejemplo:* De `2.0.0` a `3.0.0`.

2. **Incremento de MINOR (Nuevas funcionalidades):** Si añades funcionalidades nuevas compatibles con versiones anteriores, incrementa el número menor.
   - *Ejemplo:* De `2.1.0` a `2.2.0`.

3. **Incremento de PATCH (Corrección de errores):** Si realizas correcciones de errores o mejoras menores, incrementa el número de parche.
   - *Ejemplo:* De `2.2.1` a `2.2.2`.

## Importancia del Versionado Semántico en Proyectos Ágiles

En entornos ágiles, el versionado semántico es vital para comunicar el impacto de los cambios de manera clara y efectiva.

**Beneficios clave:**

1. **Comunicación clara:** Permite a cualquier miembro del equipo o cliente entender inmediatamente el tipo de actualización al observar el número de versión.

2. **Gestión de dependencias:** Ayuda a los desarrolladores a evitar actualizaciones que puedan romper sus sistemas, especialmente cuando hay incrementos en el número MAJOR.

3. **Mejora del flujo ágil:** Facilita la planificación de sprints y la organización de versiones incrementales, alineando mejor el trabajo del equipo.

## Cómo Implementar el Versionado Semántico en Proyectos Ágiles

1. **Inicializar el proyecto con SemVer:** Comienza con la versión `1.0.0` para proyectos nuevos. Si el proyecto está en fase experimental, puedes usar `0.x.x`.

2. **Versionado de APIs:** Para APIs públicas, es crucial seguir estrictamente el versionado MAJOR para evitar rupturas inesperadas en los consumidores.

3. **Integración con Agile y DevOps:** Planifica lanzamientos pequeños y frecuentes. Cada sprint puede culminar con una nueva versión MINOR o PATCH. Las actualizaciones MAJOR deben planificarse cuidadosamente.

## Versiones "Pre-release" en el Versionado Semántico

Las versiones de pre-lanzamiento permiten etiquetar versiones que aún están en desarrollo o prueba, sin afectar a la versión estable.

**Formato:** `MAJOR.MINOR.PATCH-prerelease`

**Ejemplos:**

- `1.0.0-alpha`: Versión preliminar con funcionalidades en desarrollo activo.
- `1.0.0-beta`: Versión más estable que necesita pruebas adicionales.
- `1.0.0-rc.1`: Primera versión candidata al lanzamiento final.

## Ejemplos de Versionado Semántico en el Mundo Real

1. **Node.js:** Incrementa el número MAJOR al introducir cambios incompatibles. Las versiones 14.x.x son retrocompatibles, mientras que 15.x.x puede romper compatibilidad.

2. **Angular:** Sigue estrictamente SemVer, lo que permite a los desarrolladores prever el impacto de las actualizaciones.

3. **Librerías populares:** Frameworks como React, Vue y Spring Framework utilizan SemVer, facilitando actualizaciones seguras de dependencias.

## Versionado Semántico en Scrum

El versionado semántico complementa el marco de trabajo Scrum al organizar el progreso del producto en sprints.

### Durante el Sprint Planning

- **Definir el impacto de los cambios:**
  - **MAJOR:** Cambios incompatibles o disruptivos.
  - **MINOR:** Nuevas características compatibles.
  - **PATCH:** Correcciones menores o mejoras.

### Al Final de Cada Sprint

- **Actualizar la versión según los cambios:**
  - Nuevas características → Incrementa **MINOR** (`1.0.0` a `1.1.0`).
  - Correcciones de errores → Incrementa **PATCH** (`1.1.0` a `1.1.1`).
  - Cambios incompatibles → Incrementa **MAJOR** (`1.1.1` a `2.0.0`).

- **Liberar una nueva versión del producto** para asegurar entregas incrementales y mejoras continuas.

### Versiones de Pre-release

- Utiliza sufijos como `-alpha`, `-beta`, `-rc` para versiones en desarrollo o prueba.
  - *Ejemplo:* `1.2.0-beta.1` antes del lanzamiento final.

## Flujo de Trabajo con Versionado Semántico en Scrum

1. **Desarrollo en Ramas de Funcionalidad (Feature Branches):** Asigna versiones `alpha` a nuevas funcionalidades en desarrollo (e.g., `1.1.0-alpha.1`).

2. **Revisión y Pruebas del Sprint:** Etiqueta versiones `beta` para pruebas adicionales (e.g., `1.1.0-beta.1`).

3. **Lanzamiento Final:** Después de las pruebas, libera la versión estable sin sufijos (e.g., `1.1.0`).

## Buenas Prácticas

- **Usar Etiquetas Git:** Para marcar versiones de manera precisa.

- **Automatizar con CI/CD:** Herramientas como **Semantic Release** pueden facilitar el proceso.

- **Comunicación Clara:** Indica siempre si un cambio requiere incremento de **MAJOR**, **MINOR** o **PATCH**.

## Ejemplo Práctico

- **Sprint 1:** Se añade una nueva funcionalidad.
  - Versión resultante: `1.1.0`.

- **Sprint 2:** Se corrigen errores detectados.
  - Versión resultante: `1.1.1`.

- **Sprint 3:** Se realiza un cambio de arquitectura que rompe compatibilidad.
  - Versión resultante: `2.0.0`.

Este enfoque garantiza entregas constantes y permite a los equipos y usuarios comprender fácilmente el impacto de cada actualización.