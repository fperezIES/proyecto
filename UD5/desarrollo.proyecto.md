# Desarrollo del proyecto

Llegados a este punto, se inicia el desarrollo propiamente dicho, que en líneas generales incluirá los pasos detallados en los siguientes apartados.

Cada proyecto podrá ajustar el orden, la profundidad y la forma de abordar estos pasos según la metodología elegida (Scrum, Kanban, cascada, etc.), pero es recomendable seguir este flujo general para asegurar la calidad y el éxito del trabajo.

## Integración de Git y Jira

Se debe [enlazar el repositorio del proyecto con Jira](../UD2/gitjira.md) para que los issues y el trabajo realizado pueda ser enlazado a los issues al realizar los commits.

Cada miembro del equipo debe enlazar su trabajo a Gira usado el ID del issue de Jira al inicio del mensaje del commit.

Se crearán sprints asignando al menos una tarea a cada miembro del equipo. Cada miembro debe subir el resultado de su trabajo al repositorio enlazando el commit con el issue asignado.

También se debe añadir el tiempo empleado en la tareas al issue de Jira.

## Seguimiento del tiempo

Si se usa un proyecto scrum gestionado por el equipo se deben añadir a los issues los siguientes campos para facilitar el seguimiento de las horas de trabajo dedicadas a cada issue.

Se deben habilitar los campos (En la "Configuración del proyecto" -> "Tipos de incidencias" ):

- "Estimación original"
- "Seguimiento de tiempo"

De este modo se podrá añadir una estimación inicial de tiempo que se dedicará al issue. Y también se facilitará  el seguimiento del tiempo que se ha trabajado en cada issue.

Cada miembro del equipo debe realizar el seguimiento de tiempo dedicado a cada tarea. De este modo podremos obtener informes de la evolución del esfuerzo realizado

## 1 **Análisis de requisitos** (detallado y refinado a partir de la propuesta inicial).

Análisis de requisitos detallado y refinado a partir de la propuesta inicial.  Se deben añadir los requisitos como [historias de usario](../UD1/historias_de_usuario.md) a Jira.


## 2 **Diseño** (arquitectura, diagramas, prototipos).

### 2.1 Diagramas UML

Se realizará un primer sprint de una semana, en el que cada miembro del proyecto realizará uno de los siguientes diagramas y lo subirá al repositorio enlazándolo con el issue correspondiente. 
También se debe añadir el tiempo dedicado al issue y gestionar el estado de finalización del issue.

* [Especificación UML](https://www.omg.org/spec/UML/)
* [Herramienta recomendada: Visual Paradigm Online](https://online.visual-paradigm.com/es/)

#### Diagrama de casos de uso

- Representa las interacciones entre los usuarios (actores) y el sistema.
- Muestra las funcionalidades principales del software desde el punto de vista del usuario.
- Debe incluir los actores, los casos de uso y sus relaciones (asociaciones, inclusiones o extensiones).

#### Diagrama de despliegue

- Representa la arquitectura física del sistema, indicando los nodos (servidores, bases de datos, dispositivos) y sus relaciones.
- Muestra dónde y cómo se ejecutarán los componentes del software.
- Es clave para planificar la infraestructura y distribución del sistema en distintos entornos (desarrollo, pruebas, producción).

#### Diagrama(s) de actividad

- Describe el flujo de trabajo o lógica de un proceso dentro del sistema.
- Incluye acciones, decisiones y bifurcaciones en el flujo de ejecución.
- Es útil para modelar algoritmos, procesos de negocio o el comportamiento de un caso de uso en detalle.

#### Diagrama de clases

- Representa la estructura estática del sistema, definiendo las clases, sus atributos y métodos.
- Incluye relaciones como herencia, asociación y agregación entre clases.
- Permite visualizar la organización del código antes de su implementación.
- Ayuda a comprender la modularidad y la reutilización de componentes en el sistema.

### 2.2 Mockups de UI

- Representan una vista previa visual de la interfaz de usuario antes del desarrollo.
- Permiten definir la distribución de los elementos, la navegación y la experiencia de usuario.
- Se pueden crear con herramientas como [Figma](https://www.figma.com/), [Balsamiq](https://balsamiq.com/) o [Sketch](https://www.sketch.com/).
- Facilitan la validación temprana del diseño con usuarios y partes interesadas.


### 2.3 **Esquema de base de datos**

- Modelo entidad-relación o tablas principales.
- Claves primarias y relaciones clave.

## 3 **Implementación** (programación, integración continua, control de versiones).

...

## 4 **Pruebas** (unitarias, de integración, de aceptación).

...
## 5 **Puesta en producción** (despliegue, configuración de servidores, etc.).

...
## 6 **Mantenimiento y plan de mejora** (resolución de incidencias, nuevas funcionalidades).

...
## 7 **Documentación** (manuales de uso, guías de instalación, documentación interna).

...
## 8 **Presentación** (exposición final, demo al cliente o interesados).

...