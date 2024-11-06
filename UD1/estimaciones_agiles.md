

# Estimación en Proyectos Ágiles: Puntos de Historia y Horas de Trabajo

La estimación es una práctica fundamental en la planificación de proyectos ágiles, ya que permite a los equipos prever el esfuerzo y tiempo necesarios para completar las tareas y organizar mejor los sprints. En metodologías ágiles, se utilizan principalmente dos enfoques de estimación: **puntos de historia** y **horas de trabajo**.



## ¿Qué es la Estimación?

En el contexto ágil, la estimación ayuda a medir la **complejidad**, **tamaño** o **esfuerzo necesario** para completar una historia de usuario o tarea. Esta medición no siempre es precisa, pero permite al equipo planificar de manera eficiente y ajustar su capacidad de trabajo.

Existen dos métodos principales de estimación en Scrum y otros marcos ágiles:

1. **Puntos de Historia**: miden el esfuerzo relativo de las tareas en función de la complejidad, el riesgo y el nivel de incertidumbre.
2. **Horas de Trabajo**: miden el tiempo real que los miembros del equipo esperan invertir en cada tarea.



## Puntos de Historia

### ¿Qué Son los Puntos de Historia?

Los puntos de historia son una unidad de medida que se asigna a cada historia de usuario para representar el **esfuerzo relativo** que requiere su desarrollo. No equivalen a horas o días exactos, sino que sirven como referencia para comparar tareas entre sí en función de la complejidad y el esfuerzo.

### Cómo Asignar Puntos de Historia

La asignación de puntos de historia suele realizarse usando **Series de Fibonacci** (1, 2, 3, 5, 8, 13, etc.), ya que esta escala ayuda a reflejar de forma progresiva el aumento de la incertidumbre y la complejidad.

1. **Historia muy pequeña** (p. ej., una interfaz básica): 1-2 puntos.
2. **Historia simple** pero que requiere algo de desarrollo: 3 puntos.
3. **Historia con cierta complejidad** y algunas dependencias: 5 puntos.
4. **Historia grande y compleja**: 8-13 puntos.
5. **Historia extremadamente compleja** o incierta: 20+ puntos (aunque es preferible dividirla).

### Cuándo Utilizar los Puntos de Historia

Los puntos de historia son útiles para estimar cuando:

- **Se trabaja en equipo**: permiten una visión compartida del esfuerzo.
- **Se busca medir la capacidad del equipo**: sirven para evaluar la velocidad del equipo (puntos completados por sprint).
- **Existen tareas con diferente nivel de incertidumbre**: los puntos se adaptan bien a tareas donde el esfuerzo es difícil de predecir en horas exactas.
- **Se necesita flexibilidad**: permiten adaptarse a cambios de alcance o prioridad sin basarse en horas.

### Beneficios de los Puntos de Historia

1. **Promueven el trabajo colaborativo**: el equipo acuerda en conjunto la complejidad de cada tarea.
2. **Son rápidos y menos propensos a la precisión excesiva**: ayudan a estimar de forma aproximada sin perder tiempo en detalles.
3. **Mejoran la velocidad**: conocer la velocidad del equipo (puntos por sprint) ayuda a proyectar el tiempo necesario para completar el backlog.



## Horas de Trabajo

### ¿Qué Son las Horas de Trabajo?

Las horas de trabajo son una estimación directa del tiempo necesario para completar una tarea. A diferencia de los puntos de historia, las horas pretenden ser una aproximación más precisa del esfuerzo y tiempo que requerirá una actividad, aunque siempre es una aproximación y puede ajustarse.

### Cómo Asignar Horas de Trabajo

Asignar horas de trabajo implica estimar el tiempo que cada miembro del equipo, o el equipo en conjunto, necesita para completar una tarea específica.

- **Tareas simples**: entre 1 y 3 horas.
- **Tareas moderadas**: entre 4 y 8 horas.
- **Tareas complejas**: pueden requerir de 8 horas o más, y es recomendable dividirlas si superan la duración del sprint.

### Cuándo Utilizar las Horas de Trabajo

Las horas de trabajo son útiles cuando:

- **La tarea es bien conocida y predecible**: en estos casos, los equipos pueden estimar el tiempo con precisión.
- **Se necesita una programación precisa**: cuando hay limitaciones de tiempo o el proyecto es muy ajustado en cronograma.
- **Hay trabajos individuales específicos**: tareas que dependerán de una persona en particular, como configuraciones técnicas o revisiones.
- **Existen dependencias externas**: las horas permiten organizar mejor el flujo entre tareas dependientes.

### Beneficios de las Horas de Trabajo

1. **Permiten estimaciones detalladas**: son útiles para prever tareas concretas que necesitan precisión.
2. **Mejoran la planificación individual**: los miembros del equipo pueden organizar sus jornadas de trabajo en función de tareas específicas.
3. **Útiles para proyectos con tiempos rígidos**: proporcionan un control de tiempo más detallado y ayudan a prever desviaciones en el cronograma.



## Comparación entre Puntos de Historia y Horas de Trabajo

| Característica                    | Puntos de Historia                                           | Horas de Trabajo                             |
|-----------------------------------|--------------------------------------------------------------|----------------------------------------------|
| **Medida**                        | Complejidad, esfuerzo relativo                               | Tiempo real estimado                         |
| **Precisión**                     | Menos precisa (enfoque relativo)                             | Más precisa (enfoque directo)                |
| **Uso**                           | Comparar tareas de diferentes niveles de complejidad         | Planificación detallada y tareas bien definidas |
| **Colaboración**                  | Fomenta el consenso del equipo                               | Mayormente individual                        |
| **Contexto Ideal**                | Tareas inciertas o con dificultad de medir en horas          | Tareas predecibles y con cronograma rígido   |
| **Flexibilidad**                  | Alta (permite cambios en el backlog)                         | Baja (basada en tiempos precisos)            |


## Ejemplo de Estimación en un Proyecto

Supongamos un equipo que trabaja en una aplicación de tareas pendientes. Algunas de las historias de usuario en su Product Backlog son:

1. **Como usuario, quiero crear tareas con recordatorios**.
2. **Como administrador, quiero ver estadísticas de los usuarios activos**.

En la planificación del sprint, el equipo estima cada historia:

1. La primera historia es **simple**, pero requiere cierta lógica para programar los recordatorios. Se asignan **3 puntos** o entre **4 y 6 horas** de trabajo.
2. La segunda historia es **moderadamente compleja** debido al procesamiento de datos y generación de estadísticas. Se asignan **5 puntos** o entre **8 y 10 horas**.

La elección entre puntos o horas dependerá del contexto y la cultura de estimación del equipo. En un entorno ágil, suele ser más común utilizar puntos de historia para mantener flexibilidad, mientras que las horas son útiles para tareas específicas o previsión de desviaciones en el tiempo de entrega.



# Bibliografía

- [Estimaciones en Jira](https://www.atlassian.com/es/agile/project-management/estimation)
- [Planning Poker](https://marketplace.atlassian.com/apps/1212495/planning-poker)