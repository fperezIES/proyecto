
# Historias de Usuario

Las historias de usuario son una herramienta fundamental en el desarrollo ágil de software. Aportan una forma estructurada y sencilla de representar los requisitos de usuario, enfocándose en las necesidades y objetivos que tiene un usuario final cuando utiliza el sistema. 

## ¿Qué es una Historia de Usuario?

Una historia de usuario es una descripción breve y concisa de una funcionalidad del sistema desde la perspectiva del usuario. Su objetivo principal es entender **qué quiere lograr el usuario** y **por qué lo necesita**, sin entrar en detalles técnicos de implementación.


## Estructura de una Historia de Usuario

La estructura más común para redactar historias de usuario es la siguiente:

- **Como [rol o tipo de usuario]**: define quién va a utilizar la funcionalidad.
- **Quiero [acción o funcionalidad]**: describe la acción o funcionalidad que el usuario desea.
- **Para [beneficio o valor]**: aclara el beneficio o valor que espera obtener el usuario.

**Ejemplo**:
> Como **administrador**, quiero **poder restablecer contraseñas de usuarios**, para **ayudar a los usuarios que hayan olvidado su contraseña**.


## Características de las Buenas Historias de Usuario

Para que una historia de usuario sea efectiva, se debe asegurar que cumple con las siguientes características (regla **INVEST**):

1. **Independiente**: cada historia debería ser autónoma y no depender de otras.
2. **Negociable**: debe permitir flexibilidad para discutir y ajustar detalles.
3. **Valiosa**: aporta un beneficio claro al usuario.
4. **Estimable**: es posible estimar el tiempo o esfuerzo necesario.
5. **Pequeña**: debe ser lo suficientemente breve para completarse en un sprint.
6. **Testable**: debe poder comprobarse si se ha cumplido correctamente.



## Beneficios de las Historias de Usuario

- **Enfocan el desarrollo en el usuario final**: aseguran que el software responde a las necesidades reales.
- **Fomentan la comunicación**: al ser claras y concisas, facilitan la comprensión entre desarrolladores y usuarios.
- **Promueven el desarrollo ágil**: son cortas y fáciles de modificar, permitiendo adaptarse a cambios rápidos.


## Ejemplo de Redacción

Veamos algunos ejemplos para distintos roles en una aplicación de gestión de proyectos:

1. **Como usuario**:
    - "Como **usuario registrado**, quiero **ver una lista de mis tareas pendientes** para **poder organizar mi trabajo diario**."

2. **Como administrador**:
    - "Como **administrador**, quiero **acceder a un panel de control** para **gestionar usuarios y sus permisos**."

3. **Como cliente**:
    - "Como **cliente**, quiero **consultar el estado de mis pedidos en tiempo real** para **planificar mejor mis entregas**."



## Criterios de Aceptación

Para garantizar que una historia de usuario se implemente correctamente, se establecen **criterios de aceptación**. Son condiciones que deben cumplirse para que la historia sea considerada completa y funcional.

**Ejemplo de criterios de aceptación**:
Para la historia:
> Como **usuario registrado**, quiero **ver una lista de mis tareas pendientes** para **organizar mi trabajo diario**.

Podrían ser:
- El usuario debe poder ver todas las tareas pendientes en una lista ordenada por fecha de vencimiento.
- Cada tarea debe mostrar su título, descripción y fecha límite.
- Debe haber una opción para marcar tareas como completadas.


## Buenas Prácticas en Historias de Usuario

1. **Mantener la simplicidad**: evitar descripciones largas y técnicas. Las historias deben ser claras y fáciles de entender.
2. **Enfocar en el valor**: cada historia debe responder a una necesidad o problema del usuario.
3. **Involucrar al usuario**: trabajar junto al usuario (o representante) en la redacción para asegurar que las historias reflejan sus necesidades reales.
4. **Actualizar**: si la necesidad cambia, adaptar la historia de usuario en lugar de descartarla.


---

# Gestión y Priorización de Historias de Usuario en Scrum

Dentro de Scrum, las historias de usuario son elementos clave en el **Product Backlog** y el **Sprint Backlog**, ayudando a organizar y priorizar el trabajo en función de las necesidades del usuario y del proyecto. Veamos cómo se estructuran y gestionan en cada uno de estos contextos.


## Product Backlog

El **Product Backlog** es una lista ordenada de todo el trabajo que debe realizarse para desarrollar y mejorar el producto. Aquí es donde se agrupan y priorizan las historias de usuario junto con otros requisitos del proyecto. Su gestión es responsabilidad del **Product Owner** (o propietario del producto), quien define y prioriza los elementos según el valor que aportan al usuario y a los objetivos del proyecto.

### Características de un Buen Product Backlog

Un Product Backlog bien gestionado debe:

1. **Ser visible y accesible**: todos los miembros del equipo y las partes interesadas deberían poder revisarlo.
2. **Estar ordenado por prioridad**: las historias más valiosas y urgentes deben estar al principio.
3. **Ser adaptable**: debe poder ajustarse con rapidez ante cambios en los requisitos o las prioridades del negocio.

### Priorización en el Product Backlog

Para asegurar que el equipo trabaje en lo más importante, el Product Owner usa distintas técnicas para priorizar las historias de usuario, entre ellas:

- **MVP (Producto Mínimo Viable)**: determinar qué historias de usuario son esenciales para lanzar una versión funcional básica del producto.
- **Matriz de Valor vs. Esfuerzo**: evaluar las historias en función de cuánto valor aportan frente al esfuerzo necesario para implementarlas.
- **MoSCoW (Must Have, Should Have, Could Have, Won't Have)**: clasifica las historias en "Imprescindibles", "Deseables", "Posibles" y "No necesarias en este momento".


## Sprint Backlog

El **Sprint Backlog** es el conjunto de historias de usuario seleccionadas del Product Backlog que se completarán en un sprint concreto. Esta lista es propiedad del **Equipo de Desarrollo**, que tiene la responsabilidad de desglosar cada historia en tareas y estimar el tiempo necesario para completarlas.

### Proceso de Selección para el Sprint Backlog

Durante la **Sprint Planning** (Planificación del Sprint), el equipo revisa el Product Backlog y decide cuántas historias de usuario pueden abordar en el sprint, de acuerdo con su capacidad y velocidad de trabajo. Para seleccionar las historias, se tiene en cuenta:

1. **Capacidad del equipo**: el tiempo y esfuerzo disponible en el sprint.
2. **Estimación de cada historia**: historias más grandes pueden dividirse en subtareas.
3. **Objetivos del Sprint**: asegurar que las historias seleccionadas contribuyan a alcanzar los objetivos específicos del sprint.

### Ejemplo de Selección de Historias para el Sprint Backlog

Supongamos que tenemos las siguientes historias de usuario en el Product Backlog para una aplicación de gestión de tareas:

- **H1**: Como **usuario registrado**, quiero **crear tareas con recordatorios** para **gestionar mis plazos**.
- **H2**: Como **administrador**, quiero **ver informes de actividad** para **supervisar el rendimiento de usuarios**.
- **H3**: Como **usuario registrado**, quiero **recibir notificaciones de tareas vencidas** para **no perder plazos**.

Durante el Sprint Planning, el equipo selecciona **H1** y **H3** por ser más pequeñas y alcanzar los objetivos prioritarios del usuario final. **H2** se deja para un próximo sprint, ya que requiere más tiempo de desarrollo y no es esencial para el próximo lanzamiento.

## Refinamiento del Backlog

El **Backlog Refinement** o refinamiento del Product Backlog es una reunión regular donde el equipo revisa y detalla las historias de usuario, agregando información como criterios de aceptación, dividiendo historias grandes en otras más pequeñas, y ajustando prioridades si es necesario. Esto asegura que el equipo siempre tenga historias preparadas para el siguiente sprint.

### ¿Qué se Revisa en el Refinamiento?

1. **Claridad de la Historia**: asegurar que cada historia de usuario tiene un objetivo claro y bien definido.
2. **Criterios de Aceptación**: agregar o ajustar criterios que aclaren cuándo una historia estará completa.
3. **Dividir Historias Grandes**: las historias que no pueden completarse en un sprint se dividen en historias más pequeñas.

### Ejemplo de Refinamiento

Si en el Product Backlog hay una historia de usuario como:

> "Como **usuario**, quiero **visualizar un resumen de mis actividades diarias** para **entender mi rendimiento**."

En el refinamiento, podría desglosarse en historias más pequeñas, como:

- "Como **usuario**, quiero **ver el número de tareas completadas hoy** para **evaluar mi productividad diaria**."
- "Como **usuario**, quiero **ver el tiempo promedio por tarea completada** para **mejorar mi eficiencia**."


## Beneficios de una Buena Gestión de Historias en Backlogs

1. **Flexibilidad para el cambio**: los backlogs pueden ajustarse a medida que evolucionan las necesidades.
2. **Foco en el usuario**: priorizar las historias ayuda a entregar rápidamente lo que más valor aporta.
3. **Mejor planificación del equipo**: el refinamiento y la planificación permiten que el equipo siempre tenga historias bien definidas y alcanzables.


## Bibliografía

- [Historias de usuairo Jira ](https://www.atlassian.com/es/agile/project-management/user-stories)