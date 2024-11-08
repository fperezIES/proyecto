# **Ejercicio 1: Uso de Kanban con Trello para organizar las tareas del curso durante el primer trimestre**

El objetivo de esta tarea es que aprendas a utilizar **Trello** y el método **Kanban** para organizarte mejor y gestionar tus tareas de manera más eficiente. Este ejercicio te ayudará a estructurar las actividades del curso de forma visual y controlada.


### 1. **Crea una cuenta gratuita en Trello**
   - Si no tienes cuenta, regístrate en [Trello](https://www.trello.com)
   - Una vez registrado, familiarízate con la interfaz. 

### 2. **Crea un tablero**
   - En el menú principal tienes el botón 'Crear' o en la barra que está a la izquierda donde pone 'Sus tableros' hay un + para crearlo.
   - Llama al nuevo tablero ejercicio1<nombre_alumno> 
   - Cambia la visibilidad a **Privado**
   
### 3. **Crea las siguientes listas:**
   - **Por hacer** (donde colocarás las tareas pendientes)
   - **En progreso** (tareas que estás realizando actualmente)
   - **En revisión** (cuando terminas una tarea, pero está pendiente de revisión o corrección)
   - **Completado** (tareas finalizadas)
### 4. **Crea las tarjetas (o tareas):**
- En cada una de las listas, puedes crear 'Tarjetas' que representan las tareas que hay que hacer en el proyecto.
- Por cada tarea que tengas que hacer en una asignatura del ciclo, crea una tarjeta. Para empezar, puedes añadir las tareas de esta semana.
- **Cada tarjeta debe incluir:**
    - Nombre de la tarea: Un título que describa claramente la actividad.
    - Breve descripción: Explica en una o dos frases en qué consiste la tarea.
    - Fecha de vencimiento: Indica cuándo debe estar completada la tarea.
    - Prioridad: Asigna una prioridad dependiendo de la urgencia o importancia (está en campos personalizados). 
    - También puedes utilizar etiquetas o colores para diferenciarlas.

### 4. **Trabajo a realizar con las tarjetas:**
- De las tareas pendientes, asigna alguna (más urgente o fecha más cercana de finalización) a un usuario (en principio a ti mismo)
- Estas tarjetas hay que pasarlas al panel ‘En progreso’
- Añade alguna tarjeta con alguna tarea ya finalizada y que esté pendiente de revisión por parte del profesor y pásala al panel ‘En revisión’
- Añade alguna tarjeta con una tarea finalizada y revisada. Márcala como completada y pásala al panel ‘Completado’
- Por último, añade como miembro a tu profesor (<profe>@iessanvicente.com). Esto permitirá a tu profesor ver el progreso de tu trabajo.
- Asígnale una tarea: Crea una tarea llamada ‘Revisión ejercicio 1 Kanban’ y asígnasela para que pueda revisarla o darte feedback y marcarla como finalizada.

---
# **Ejercicio 2: Uso de Kanban con Trello para organizar las tareas de la construcció de un proyecto software web**

En este ejercicio, vamos a simular el desarrollo de un proyecto software utilizando la metodología Kanban.

Suponemos que un equipo de trabajo ha realizado la toma de requisitos y establecido las diferentes tareas que tenemos que hacer en nuestro equipo y solamente nos preocuparemos del desarrollo del software como de la realización de las pruebas de funcionamiento.

### 1. **Descripción de la aplicación:**

Nos han encargado desarrollar una tienda online de ropa, dicha tienda, contendrá diferentes productos organizados por categorías. Sobre los productos que existen, unos tendrán stock y otros no pero guardaremos referencia de ellos porque o bien se han acabado o porque no hemos pedido nada todavía a la fábrica. 

Los usuarios (registrados o no) podrán ver los artículos que haya stock y añadirlos al carrito de compra. 

Los usuarios del back podrán manipular los artículos (crearlos y modificarlos) y crear las diferentes categorías a la que pertenecerán los artículos, también podrán ver informes estadísticos de los artículos y las ventas. 

Por último, podemos indicar que cualquier persona se podrá registrar como usuario del front y que solamente podrá realizar compras de productos.

El equipo de diseño nos ha pasado las siguientes tareas a realizar y el tiempo estimado que necesitaremos para realizarlas:
- T01	Creación de la página principal del proyecto, así como de la definición de los estilos que se utilizarán en todas las páginas. (2 días)
- T02	Creación de la base de datos, tanto las tablas de información como de los diferentes roles de los usuarios (1 día)
- T03	Creación del formulario para crear categorías (1 día)
- T04	Creación del formulario de alta de artículos (2 días)
- T05	Creación de la página que muestra los artículos que verán los clientes o usuarios del front (solamente los que tengan stock) (1 día)
- T06	Creación de la página que muestra todos los artículos existentes para los usuarios del back (1 día)
- T07	Creación del formulario para modificar los artículos (1 día)
- T08	Creación de filtros para aplicar en las páginas que muestran los artículos (3 días)
- T09	Creación del carrito de compra y adaptación a la página donde los clientes ven los artículos (2 días)
- T10	Creación del formulario de alta de usuarios (2 días)

Por otra parte, debemos tener en cuenta que no se puede realizar ciertas tareas mientras no se hayan realizado otras, así que establecemos las siguientes dependencias:

    -	T03, T04 -> T02	Las tareas T03 y T04 no se pueden realizar mientras no esté la T02
    -	T04 -> T03
    -	T05 -> T04
    -	T06 -> T04
    -	T07 -> T04
    -	T08 -> T05, T06
    -	T09 -> T05
    -	T10 -> T02

### 2. **Trabajo a realizar:***
-	Entra en trello.com y crea un nuevo proyecto llamado ejercicio2<nombre> (donde nombre será tu nombre)
-	Añade a tu proyecto al profesor para que pueda acceder a tu trabajo (dsanchez@iessanvicente.com)
-	Crea las listas:
    -	**Por hacer** (donde colocarás las tareas pendientes)
    -	**En progreso** (tareas que estás realizando actualmente)
    -	**En revisión** (cuando terminas una tarea, pero está pendiente de revisión o corrección)
    -	**Completado** (tareas finalizadas pendientes de validación por el cliente)
    -	**Validadas por cliente** (tareas finalizadas y que el cliente las ha dado por buenas)
-	Crea tarjetas (tareas): En el tablero ‘Por hacer’, crea una tarjeta por cada tarea definidas en el enunciado del ejercicio (T01, T02, …). 
    -	Para el título, poner el detalle de la tarea con su código T01, …
    -	En la descripción escribir el texto necesario que explique en qué consiste el trabajo.
    -	No poner fecha de vencimiento
    -	Añadimos el campo ‘priority’ y en un principio ponemos todas a ‘Medium’
    -	Añadimos el campo ‘effort’ donde indicamos la duración de la tarea
    -	Añadimos un campo personalizado que creamos nosotros llamado ‘Dependencia’ y donde pondremos las tareas que dependen de ésta para poder realizarla.
-	Funcionamiento del Kanban:
    -	Los lunes, a primera hora, cada miembro del equipo cogerá una de las tarjetas asignándosela como miembro y la pasará al tablero ‘En progreso’
    -	Cuando la finalice, la pasará al tablero ‘En revisión’. 
        - Estas tareas también las debe coger un miembro del equipo diferente al que la realizó para realizar pruebas de validación y comprobación de que no contienen errores. 
        -	Todas estas pruebas durarán 1 día.
        -	Cuando estén validadas, se pasarán a ‘Completado’
    -	Para desarrollar el proyecto, tendremos en cuenta que todos los viernes se realizará una reunión con el cliente y se le entregará una nueva versión de la aplicación con al menos una funcionalidad nueva.
        -	En la reunión, el cliente nos validará la nueva versión (pasando las tarjetas aprobadas a ‘Validada’ y añadiendo la fecha de finalización de la tarea marcándola como completada), podrá proponer tanto cambios en el trabajo realizado como plantear nuevos requisitos que no estaban.
        -	Si alguna tarea no la validara el cliente, la pasaremos a la tarjeta ‘por hacer’ y apuntaremos en la descripción las indicaciones de lo que hay que hacer. Además, se cambiará la prioridad como ‘Alta’
        -	Para las nuevas funcionalidades, se crearán tarjetas de tareas y se colocarán en el tablero ‘Por hacer’

### 3. **Trabajo para entregar en Aules:**
- Vamos a simular que el equipo de trabajo consta de 2 miembros, el alumno y añadirá al profesor de la clase (o se creará otro usuario con otra cuenta), aunque toda la operativa la realizará el alumno simulando el trabajo de los 2 miembros.
-	**Diario:** Como simularemos el trabajo de cada día, vamos a crear un diario (documento) donde se apuntará cómo quedan los tableros cada día y se pueda ver la evolución del proyecto. Se pondrá un volcado de pantalla y los comentarios necesarios.
-	**Semanal:** También, se creará otro documento donde se anotará las diferentes presentaciones que se entregarán al cliente cada viernes (versiones) especificando qué funcionalidades (tareas) contienen y cuales se han rechazado.
-	**Final:** Cuando esté finalizado el proyecto software, contesta a las siguientes preguntas:
    - ¿Cuántas semanas ha durado el desarrollo del proyecto?
    -	¿Todas las semanas se han presentado al cliente algún requisito nuevo?
    -	¿En algún momento alguno de los miembros se ha quedado sin trabajar porque había alguna tarea pendiente de hacer y ésta dependía de que se haya terminado otra para poder hacerla?
    - ¿Crees que es una metodología óptima para la organización del desarrollo del software?

Estos **tres documentos** se entregarán en Aules.



