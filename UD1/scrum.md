# SCRUM 

## ¿Qué es Scrum?

Scrum es un marco de trabajo ágil que se puede utilizar para abordar proyectos complejos. Su objetivo es facilitar la colaboración entre equipos y mejorar la entrega de productos de manera incremental y continua, permitiendo a los equipos ser más ágiles y adaptarse a los cambios.

Este marco de trabajo se puede aplicar tanto en proyectos de desarrollo de software como en proyectos de sistemas o de otros ámbitos. 

## Pilares de Scrum

Scrum se basa en tres pilares fundamentales:

1. **Transparencia**: Todos los aspectos del proceso de desarrollo deben ser visibles para todos los miembros del equipo. Esto significa que el trabajo, el progreso y los obstáculos deben ser claros para el equipo y los interesados. La transparencia ayuda a fomentar la confianza y la colaboración.

2. **Inspección**: Se deben realizar inspecciones regulares a través de reuniones, para evaluar el progreso y la calidad del trabajo. La inspección permite identificar problemas y áreas de mejora, asegurando que el equipo se mantenga en el camino correcto.

3. **Adaptación**: El equipo debe ser capaz de adaptar su enfoque y procesos en función de lo que se ha aprendido durante las inspecciones. Si se detecta que algo no está funcionando como se esperaba, el equipo debe ser flexible y estar dispuesto a realizar cambios para mejorar continuamente.

## Roles en Scrum

Un equipo Scrum está compuesto por un Scrum Master, un Product Owner y el Equipo de Desarrollo. El equipo Scrum debe ser lo suficientemente pequeño como para mantenerse ágil y lo suficientemente grande como para completar un trabajo significativo dentro de un Sprint. Generalmente, suelen estar formados por 10 personas como máximo.

En el equipo Scrum no hay sub-equipos ni jerarquías. Es un conjunto de profesionales centrado en un objetivo en común: el **Product Goal** (Objetivo del Producto). El equipo Scrum debe ser multifuncional, lo que significa que deben tener todas las habilidades necesarias para crear valor en cada Sprint. También son autogestionados, lo que significa que deciden internamente quién hace qué, cuándo y cómo.

1. **Product Owner (Propietario del Producto)**: El Product Owner es el responsable de definir y priorizar los requisitos del proyecto que se va a desarrollar. Para ello, actúa como enlace entre el equipo de trabajo y el cliente o destinatario del proyecto. Puede ser parte de la empresa del cliente o incluso alguien del propio equipo de trabajo. 
El Producto Owner es el responsable de maximizar el valor del producto que se está desarrollando, intentando que el equipo no haga más tareas sino las taras que aporten más valor al proyecto.  Esto lo logra gestionando el **Product Backlog**, que es una lista priorizada de las características, mejoras y correcciones que se necesitan en el producto.
Para que el Product Owner tenga éxito, toda la organización debe respetar sus decisiones. Las decisiones del Product Owner son visibles en el contenido y el orden del Product Backlog, y los desarrolladores solo deben trabajar con los elementos del Product Backlog que provengan del Product Owner.

2. **Scrum Master**: Su principal tarea es asegurarse de que el equipo siga las prácticas y principios de Scrum. Esto incluye ayudar a eliminar obstáculos que puedan impedir el progreso del equipo y fomentar un ambiente de trabajo colaborativo y productivo. No es un jefe de proyecto o coordinador, puesto que el equipo debe autogestionarse sólo, es un miembro igualitario del equipo.

3. **Equipo de desarrollo**: El equipo de desarrollo es el responsable de crear el producto. Para ello, debe determinar cómo se va a realizar el trabajo y desarrollarlo. Este equipo debe ser multifuncional, debe tener todas las habilidades necesarias para el desarrollo del producto.


## Proceso Scrum

### Backlog (Lista de requerimientos)
Inicialmente, el Product Owner se encarga de recopilar los requisitos del proyecto a través de historias de usuario. Una histora de usuario es la descripción de una funcionalidad que se debe implementar en el proyecto. Cada historia debe ser comprensible y concreta, para que el equipo pueda implementarla en pocas semanas. Se les pide a los usuarios de la empresa cliente que escriban lo que esperan de cada funcionalidad. 

El conjunto completo de historias se recopila en una colección llamada **Product Backlog**. De este backlog, algunas historias formarán finalmente parte de la aplicación y otras serán descartadas.

Es importante destacar que el backlog es una lista dinámica que se irá actualizando a lo largo del desarrollo del proyecto, pudiéndose introducir, eliminar o modificar funcionalidades ya existentes.

Un ejemplo de historia de usuario puede estar formado por los siguientes campos: nombre, descripción de la historia, prioridad y estimación de esfuerzo.


### Sprints

Un sprint o iteración es un periodo de tiempo fijo en el que se debe obtener una entrega del proyecto que proporcione valor. Un sprint suele durar entre 1 y 4 semanas y en cada sprint se deben añadir algunas de las funcionalidades extraídas del backlog.

A cada historia de usuario en el backlog se le asigna un tiempo, generalmente en horas, días o incluso semanas. Así, el tiempo total estimado de un sprint es la suma de todas las historias de usuario seleccionadas para ese sprint.
Para determinar si el tiempo estimado total difiere mucho del tiempo real, podemos usar algunas herramientas adicionales, como los gráficos de quemado (burndown charts), que nos ayudan de manera gráfica a determinar qué medidas se pueden tomar para reducir esta diferencia.

![Burndown chart](img/burndown_charts.png){:class="center"}
### Sprint Planning (Reunión de planificación)

Al comenzar cada iteración, se realiza una reunión de planificación con todo el equipo, donde el Product Owner indica qué funcionalides se espera que se entreguen al finalizar esa iteración y con qué prioridad. 

El equipo completo decide qué requerimientos com mayor prioridad del backlog se pueden realizar en esa iteración y se planifica su desarrollo para que termine en la fecha final de ese sprint. Para poder planificar su desarrollo es importante desglosar cada tarea en tareas más pequeñas y determinar si una tarea depende de la realización de otra. En esta misma reunión se puede decidir qué tareas sea asignan a cada miembro del equipo.

Durante la iteración, el backlog se congela, es decir, no podemos cambiar ningún requisito anterior hasta que comience la siguiente iteración. Tampoco se puede modificar la fecha final de ese sprint.

En esta reunión, el Scrum Master es el encargado de asegurarse de que el equipo comprende que se espera obtener al final de la iteración y que disponen de todo lo necesario para completar su trabajo.


### Daily Scrum (Reunión diaria)

Es una reunión breve que se realiza todos los días, generalmente por la mañana. Su objetivo principal es que los miembros del equipo compartan información sobre el progreso de su trabajo. Para ello, cada miembro del equipo debe responder a tres preguntas clave:

1. ¿Qué hice ayer? - Qué trabajo se ha realizado desde la última reunión.
2. ¿Qué haré hoy? - Indicar el trabajo que se va a realizar hasta la siguiente sesión.
3. ¿Hay algún impedimento? - Se discuten los obstáculos o problemas que podrían estar bloqueando el progreso.

Se recomienda que la reunión se realice todos los días en el mismo lugar a la misma hora, que sea breve, de unos 15 minutos, y que se realice de pie para mantenerla ágil y enfocada. Es una forma de fomentar la comunicación y la colaboración dentro del equipo. 

El Scrum Master es el responsable de que la reunión no exceda el tiempo establecido y de informar sobre el estado de los problemas detectados al Product Owner para que tome las decisiones oportunas.

Las ventajas de realizar esta reunión diaria son numerosas:

1. Comunicación constante: Fomentan la comunicación abierta entre los miembros del equipo, lo que ayuda a mantener a todos informados sobre el progreso y los obstáculos encontrados.

2. Identificación temprana de problemas: Al discutir lo que cada uno ha hecho, lo que planea hacer y cualquier impedimento, se pueden identificar y abordar problemas rápidamente antes de que se conviertan en obstáculos mayores.

3. Alineación del equipo: Ayudan a asegurar que todos estén alineados con los objetivos del sprint y comprendan las prioridades del día.

4. Responsabilidad: Cada miembro del equipo se siente más responsable de su trabajo, ya que comparte su progreso y compromisos con el grupo.

5. Mejora continua: Estas reuniones ofrecen una oportunidad para reflexionar sobre el proceso y hacer ajustes en tiempo real, lo que fomenta la mejora continua.

6. Motivación: Ver el progreso de los demás puede ser motivador y crear un sentido de camaradería dentro del equipo.


### Sprint Review (Revisión del Sprint)

La Revisión del Sprint es la reunión que se lleva a cabo al final de cada sprint. En esta reunión, el equipo de desarrollo presenta el trabajo completado durante el sprint a los interesados y al Product Owner.

El Product Owner se encarga de validar si el trabajo realizado por el equipo cumple con los objetivos del sprint. Además podrá proponer mejoras o modificaciones que deberán reflejarse en la lista de requerimientos (backlog) para siguientes sprints.

Esta reunión también es un momento idóneo paa recibir retroalimentación de los interesados, lo que puede ayudar a ajustar el rumbo del proyecto y priorizar el trabajo futuro.


### Sprint Retrospective (Retrospectiva del Sprint)

Es una forma de autoevaluar el proceso de trabajo del equipo. Se puede realizar al finalizar un sprint o cada 2-3 sprints. 

El objetivo principal de la retrospectiva es identificar cómo ha actuado el equipo en el sprint, qué  problemas han surgido y si se han afrontado de forma correcta. Al final de la reunión, el equipo debe obtener un plan de mejora para el próximo sprint. Es un espacio seguro donde todos los miembros del equipo pueden compartir sus pensamientos y sugerencias, fomentando la comunicación abierta y la colaboración.

---

### Ejercicio 1:

En [este video](https://www.youtube.com/watch?v=XU0llRltyFM)  tienes un resumen del marco de trabajo Scrum. Después de verlo, intenta responder a las siguientes preguntas:

- ¿Qué es un sprint en Scrum?
- ¿Quién es el encargado de priorizar las tareas a realizar en cada sprint?
- ¿Cómo se puede calcular la fecha final de entrega de un sprint?





