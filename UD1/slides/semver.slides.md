<!-- .slide: data-background="#2C3E50" -->
# Versionado Semántico

---

## ¿Qué es el Versionado Semántico?

- Convención de versionado con formato `MAJOR.MINOR.PATCH`.
- Propuesto por Tom Preston-Werner en 2013.
- Refleja la evolución del software y su compatibilidad con versiones anteriores.

---

## Desglose de la Notación

- **MAJOR (Versión Mayor):**
  - Incremento cuando hay cambios incompatibles.
  - Ejemplo: Cambios en la API que requieren modificaciones en el código dependiente.

- **MINOR (Versión Menor):**
  - Incremento al añadir nuevas funcionalidades compatibles.
  - Los usuarios pueden actualizar sin cambios adicionales.

- **PATCH (Parche o Corrección):**
  - Incremento al corregir errores o hacer mejoras menores.
  - No afecta la compatibilidad ni añade nuevas funcionalidades.

---

## Ejemplo de Versión: 2.3.4

- **2**: Segunda versión mayor.
- **3**: Tercera actualización de nuevas funcionalidades.
- **4**: Cuarta corrección de errores o ajustes menores.

---

## Reglas del Versionado Semántico

1. **Incremento de MAJOR (Cambios Incompatibles):**
   - Cambios que rompen compatibilidad.
   - *Ejemplo:* De `2.0.0` a `3.0.0`.

--

2. **Incremento de MINOR (Nuevas Funcionalidades):**
   - Funcionalidades nuevas compatibles con versiones anteriores.
   - *Ejemplo:* De `2.1.0` a `2.2.0`.

--

3. **Incremento de PATCH (Corrección de Errores):**
   - Correcciones de errores o mejoras menores.
   - *Ejemplo:* De `2.2.1` a `2.2.2`.

---

## Importancia en Proyectos Ágiles

- **Comunicación Clara:**
  - Permite entender el tipo de actualización de inmediato.

- **Gestión de Dependencias:**
  - Evita actualizaciones que puedan romper sistemas al revisar cambios MAJOR.

- **Mejora del Flujo Ágil:**
  - Facilita la planificación y organización de sprints y versiones.

---

## Implementación en Proyectos Ágiles

1. **Inicializar con SemVer:**
   - Comenzar con `1.0.0` o `0.x.x` si es experimental.

--

2. **Versionado de APIs:**
   - Seguir estrictamente el incremento MAJOR para APIs públicas.

--

3. **Integración con Agile y DevOps:**
   - Planificar lanzamientos frecuentes.
   - Sprints culminan con versiones MINOR o PATCH.
   - Actualizaciones MAJOR requieren planificación detallada.

---

## Versiones "Pre-release"

- **Formato:** `MAJOR.MINOR.PATCH-prerelease`

- **Usos:**
  - Etiquetar versiones en desarrollo o prueba.
  - No afectan la versión estable.

--

## Ejemplos de Pre-release

- **1.0.0-alpha:**
  - Funcionalidades en desarrollo activo.

- **1.0.0-beta:**
  - Versión más estable pero necesita más pruebas.

- **1.0.0-rc.1:**
  - Primera candidata al lanzamiento final.

---

## Ejemplos en el Mundo Real

- **Node.js:**
  - Incrementa MAJOR para cambios incompatibles.
  - Versiones 14.x.x vs. 15.x.x.

--

- **Angular:**
  - Sigue estrictamente SemVer.
  - Facilita entender el impacto de actualizaciones.

--

- **Librerías Populares:**
  - React, Vue, Spring Framework.
  - Uso de SemVer para actualizaciones seguras.

---

## Versionado Semántico en Scrum

### Durante el Sprint Planning

- **Definir Impacto de Cambios:**
  - **MAJOR:** Cambios incompatibles.
  - **MINOR:** Nuevas características compatibles.
  - **PATCH:** Correcciones menores.

--

### Al Final de Cada Sprint

- **Actualizar Versión:**
  - Nuevas características → Incrementar MINOR.
  - Correcciones de errores → Incrementar PATCH.
  - Cambios incompatibles → Incrementar MAJOR.

- **Liberar Nueva Versión:**
  - Garantiza entregas incrementales y mejoras continuas.

--

### Uso de Versiones Pre-release

- **Sufijos:** `-alpha`, `-beta`, `-rc`
- **Ejemplo:** `1.2.0-beta.1` para pruebas antes del lanzamiento final.

---

## Flujo de Trabajo con SemVer en Scrum

1. **Desarrollo en Ramas de Funcionalidad:**
   - Asignar versiones `alpha` (e.g., `1.1.0-alpha.1`).

--

2. **Revisión y Pruebas:**
   - Etiquetar versiones `beta` (e.g., `1.1.0-beta.1`).

--

3. **Lanzamiento Final:**
   - Liberar versión estable sin sufijos (e.g., `1.1.0`).

---

## Buenas Prácticas

- **Usar Etiquetas Git:**
  - Para marcar versiones de forma precisa.

- **Automatizar con CI/CD:**
  - Herramientas como Semantic Release.

- **Comunicación Clara:**
  - Indicar si un cambio es MAJOR, MINOR o PATCH.

---

## Conclusiones

- **Entregas Constantes:**
  - Al final de cada sprint, hay una nueva versión.

- **Comprensión del Impacto:**
  - Facilita entender el alcance de cada actualización.

- **Mejora Continua:**
  - Promueve la entrega incremental de valor.

