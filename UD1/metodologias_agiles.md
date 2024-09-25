# Metodologías de software


## Metodologías ágiles

Desarrollar productos de software no es una tarea fácil, por lo que existen diferentes metodologías que podemos seguir para este desarrollo. Una metodología es un conjunto de técnicas y métodos que nos ayudan a enfrentar cada etapa de un ciclo de vida. De esta manera, podemos:

- Optimizar el proceso y el producto final.
- Utilizar protocolos guiados para la planificación y el desarrollo.
- Establecer qué hacer, cómo hacerlo y cuándo, a lo largo de todo el proyecto.

Las metodologías tradicionales son realmente útiles para proyectos grandes (en términos de tiempo y presupuesto), pero tienen algunas desventajas para proyectos no tan grandes, o con un plazo cercano, o con requisitos inciertos. Por ejemplo, producen demasiada documentación y están sobreplanificadas.

Para enfrentar estos otros proyectos, muchos equipos han probado metodologías ágiles, que son especialmente adecuadas para proyectos pequeños, que se desarrollan en un corto período de tiempo y con equipos compuestos por menos de 10 personas. Con estas metodologías, promovemos el trabajo en equipo, nuestra propia responsabilidad, las necesidades del cliente y los objetivos de su empresa. La comunicación cara a cara entre los miembros del equipo y con el cliente es muy regular. De esta manera, los miembros del equipo comparten sus progresos y problemas, y reciben una retroalimentación rápida del cliente.

Para cumplir su propósito, el desarrollo ágil realiza pequeños incrementos del proyecto, con una planificación mínima. Cada incremento realiza una iteración completa sobre las etapas del software (requisitos, diseño, implementación, pruebas...), en un corto período de tiempo (generalmente de 1 a 4 semanas), conocido como *timebox*. De esta manera, minimizamos el riesgo general y el proyecto puede adaptarse a muchos cambios a lo largo de su desarrollo. La documentación solo se genera cuando realmente se necesita, y el objetivo es obtener un prototipo funcional después de cada iteración, aunque tenga funcionalidades realmente reducidas.

## 1. El Manifiesto Ágil
El Manifiesto Ágil es una especificación creada en 2001 que reúne los principales principios que una metodología debe tener para permitir que el equipo construya un proyecto de software de manera rápida y enfrentando los cambios que pueda tener en el futuro. Algunos de los principios más importantes son:
- Las personas son el principal factor de éxito de un proyecto. Es mejor crear un buen equipo y permitir que configure su propio entorno de trabajo, que construir el entorno y obligar al equipo a adaptarse a él.
- No debemos producir ninguna documentación a menos que sea necesaria para tomar una decisión de inmediato.
- Debe haber una interacción constante entre el cliente y el equipo de trabajo.
- La capacidad de enfrentar los cambios que el proyecto pueda tener durante el desarrollo es más importante que seguir una planificación rígida desde el principio.
- La principal prioridad es satisfacer al cliente a través de la entrega continua de software funcional.
- La conversación cara a cara es el método más eficiente para transmitir información en un equipo de trabajo.
- Simplicidad.

## 2. Algunas prácticas habituales

Además de los principios recogidos en el manifiesto ágil, algunas metodologías ágiles utilizan ciertas prácticas adicionales. Veamos algunas de ellas.

### **Programación en pareja (PP)**

La programación en pareja es una técnica que ofrece muchas ventajas. Dos programadores trabajan juntos en el mismo ordenador. Uno de ellos escribe el código (conductor) y el otro revisa lo que se escribe (observador). Ambos intercambian sus roles frecuentemente (por ejemplo, cada 30 minutos). El observador se encarga de guiar el trabajo del conductor y de aportar ideas para resolver posibles problemas futuros.

#### Las principales ventajas de esta técnica son:

- Se producen programas más cortos, con menos errores y mejor diseñados (ya que el código debe ser legible para ambos miembros del equipo).
- Es útil para el aprendizaje, si uno de los miembros tiene mucha experiencia y el otro es un novato, o si ambos tienen conocimientos diferentes que pueden intercambiarse.
- Si uno de los miembros deja el equipo, otro puede ocupar su lugar con el apoyo del anterior miembro, de modo que no es necesario modificar los plazos de entrega.
- Hay menos interrupciones durante el proceso, ya que ambos miembros intercambian sus tareas y pueden trabajar de manera más continua.

#### Sin embargo, también tiene algunos inconvenientes:

- Algunos ingenieros prefieren trabajar solos.
- Un novato puede sentirse intimidado si trabaja con alguien más experimentado, y viceversa (los trabajadores con experiencia pueden aburrirse ayudando a un novato).
- Es más costoso (hay que pagar dos salarios por un solo trabajo).
- Puede haber hábitos de trabajo molestos en el equipo.

### **Desarrollo guiado por pruebas (TDD)**

Esta es una técnica que utiliza iteraciones cortas basadas en casos de prueba previamente escritos. De esta manera, cada iteración produce el código necesario para pasar estas pruebas, y una vez que se pasan, se integra este código con el anterior y se optimiza. El proceso es el siguiente:

1. Añadimos una nueva prueba al conjunto actual.
2. Escribimos el código para pasar esta última prueba.
3. Ejecutamos nuevamente el conjunto de pruebas y verificamos que todas se pasen.
4. Refactorizamos el código final para optimizarlo.
5. Volvemos al paso 1.

Es importante tener un conjunto de pruebas unitarias que puedan ejecutarse automáticamente, de modo que podamos añadir más pruebas de vez en cuando y relanzarlas en cualquier momento. Veremos más adelante en este módulo algunas técnicas para definir casos de prueba y conjuntos de pruebas.

La idea principal es definir las pruebas que el sistema debe pasar antes de escribir el código correspondiente, asegurándonos de que la aplicación puede verificarse y definiendo pruebas para cada funcionalidad. De esta manera, evitamos escribir código innecesario (esto es, código que no está asociado a ninguna prueba).



## 3. Marcos de trabajo ágiles.

A continuación vamos ver dos ejemplos marcos de trabajo ágiles que se pueden utilizar para el desarrollo de proyectos completos:

- [Scrum](./scrum.md)
- [Kanban](./kanban.md)
- DevOps




