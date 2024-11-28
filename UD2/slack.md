## Introducción a Slack y su uso en el trabajo en equipo


![Logo Slack](img/Slack_logo.png){:style="width: 30%;" class="center"}

### ¿Qué es Slack?

[Slack](https://slack.com/) es una plataforma de comunicación y colaboración diseñada para facilitar el trabajo en equipo, especialmente en entornos profesionales. Combina funcionalidades de mensajería instantánea, intercambio de archivos, integración con otras herramientas y gestión de proyectos, todo en un solo lugar. Su objetivo principal es mejorar la productividad y la coordinación entre los miembros de un equipo, sustituyendo o complementando el uso de correos electrónicos y otras aplicaciones.

### ¿Por qué es útil en el mundo laboral?

En los entornos laborales actuales, especialmente en equipos distribuidos o remotos, es esencial contar con herramientas que permitan:

1. **Comunicación en tiempo real:** Slack facilita mantener conversaciones rápidas y claras.
2. **Organización del trabajo:** Permite organizar las discusiones y tareas en canales específicos.
3. **Acceso centralizado a recursos:** Los archivos, mensajes y herramientas integradas están disponibles desde un único lugar.
4. **Integración con otras herramientas:** Slack se conecta con aplicaciones como Google Drive, Trello, Jira, GitHub, Zoom, y muchas más, simplificando los flujos de trabajo.

### Funcionalidades principales de Slack

1. **Canales:**
    
    - Los canales son espacios de conversación organizados por tema, proyecto, equipo o cualquier criterio relevante.
    - Ejemplo: `#proyecto-marketing`, `#soporte-tecnico`, `#anuncios-generales`.
2. **Mensajes directos (DM):**
    
    - Comunicación privada entre dos o más personas. Ideal para conversaciones rápidas o sensibles.
3. **Búsqueda avanzada:**
    
    - Slack guarda todo el historial de mensajes, permitiendo buscar información pasada fácilmente.
4. **Compartición de archivos:**
    
    - Los usuarios pueden compartir documentos, imágenes, enlaces y otros archivos directamente en los canales o mensajes.
5. **Integraciones:**
    
    - Conecta Slack con herramientas como Asana, Jenkins, Jira, entre otras, para recibir actualizaciones automáticas.
6. **Notificaciones personalizables:**
    
    - Configura alertas según tus prioridades, evitando distracciones innecesarias.

### ¿Cómo se usa Slack en el trabajo en equipo?

1. **Gestión de proyectos:**
    
    - Crea canales específicos para cada proyecto donde los miembros del equipo puedan discutir, compartir archivos y recibir actualizaciones.
2. **Comunicación interna:**
    
    - Reduce la cantidad de correos electrónicos con mensajes rápidos y centralizados.
3. **Colaboración remota:**
    
    - Permite mantener una comunicación fluida entre equipos distribuidos en diferentes ubicaciones.
4. **Seguimiento de tareas:**
    
    - Usa integraciones con herramientas de gestión para recibir actualizaciones y mantener al equipo informado.
5. **Fomentar la cultura del equipo:**
    
    - Crea canales informales para charlas sociales (`#random`, `#memes`), fortaleciendo los lazos entre los miembros.

### Buenas prácticas para usar Slack

- **Evita la sobrecarga de canales:** Organiza los canales por temas claros y relevantes.
- **Respeta el tiempo de los demás:** Usa las menciones (@usuario) solo cuando sea necesario y ajusta tus mensajes según la urgencia.
- **Mantén la profesionalidad:** Aunque Slack permite un tono informal, recuerda que sigue siendo una herramienta laboral.
- **Documenta decisiones importantes:** Registra acuerdos clave o resúmenes en los canales correspondientes para que sean accesibles a todos.


## Integración de Slack con Jira

Slack y Jira, cuando se integran, forman una poderosa combinación para gestionar proyectos, comunicar avances y resolver problemas de manera más eficiente. Esta integración permite a los equipos estar siempre informados sobre cambios, asignaciones o incidencias en Jira sin salir de Slack.


### **¿Qué permite la integración de Slack con Jira?**

La integración entre Slack y Jira conecta los flujos de trabajo para que los equipos puedan:

1. **Recibir notificaciones en tiempo real:**
    
    - Avisos sobre nuevas incidencias, cambios de estado o actualizaciones relacionadas con tareas de Jira en canales o mensajes directos específicos de Slack.
2. **Realizar acciones desde Slack:**
    
    - Crear, asignar, comentar o actualizar tareas sin necesidad de abrir Jira.
    - Ejemplo: "Crear una incidencia en el proyecto `PROYECTO` para revisar el servidor de producción."
3. **Seguimiento centralizado:**
    
    - Agrega actualizaciones específicas de Jira a canales de Slack relacionados con un proyecto o equipo.
4. **Menor cambio de contexto:**
    
    - Consulta detalles de una tarea de Jira directamente en Slack sin necesidad de cambiar de aplicación.
5. **Colaboración mejorada:**
    
    - Comparte incidencias o historias directamente en un canal para discutirlas con el equipo.

---

### **Principales funcionalidades disponibles tras la integración**

1. **Visualización de tickets:**
    
    - Al compartir un enlace de Jira en Slack, este genera automáticamente un resumen con el estado, asignado, prioridad y descripción del ticket.
2. **Comandos directos de Jira en Slack:**
    
    - Usa comandos como `/jira create` para generar incidencias rápidamente desde Slack.
    - Otros comandos incluyen `/jira list` para ver tareas asignadas o `/jira search` para buscar tickets.
3. **Notificaciones configurables:**
    
    - Personaliza qué tipo de eventos generan notificaciones en Slack, como:
        - Cambios de estado (De "Pendiente" a "En Progreso").
        - Incidencias nuevas asignadas.
        - Comentarios en tareas específicas.
4. **Automatización:**
    
    - Usa reglas para enviar notificaciones automáticas a canales relevantes cuando:
        - Se cierra una incidencia.
        - Se alcanza una fecha límite.
        - Se crea un ticket de alta prioridad.
5. **Integración bidireccional:**
    
    - Las interacciones realizadas en Slack (como agregar un comentario) se reflejan automáticamente en Jira, asegurando la sincronización de datos.

---

### **Cómo configurar la integración Slack-Jira**

1. **Habilitar desde Jira:**
    
    - En Jira, en tu proyecto ve al menú  "Aplicaciones" → "Explorar más aplicaciones" y busca e instala  "**Jira Cloud for Slack**".
    - Sigue las instrucciones para conectar tu espacio de trabajo de Slack.
2. **Añadir el bot de Jira a Slack:**
    
    - Instala la aplicación de Jira desde el directorio de aplicaciones de Slack.
    - Autoriza la conexión entre Jira y Slack mediante tu cuenta de Jira.
3. **Configurar notificaciones:**
    
    - En el canal de Slack, escribe `/jira connect` y selecciona el proyecto de Jira que quieres vincular.
    - Define los eventos de los que deseas recibir notificaciones.
4. **Personalizar los permisos:**
    
    - Configura quién puede ver y gestionar las integraciones para garantizar la seguridad de los datos.

---

### **Ventajas de la integración**

- **Ahorro de tiempo:** Realiza acciones simples de Jira sin salir de Slack.
- **Mejor comunicación:** Mantén a todos los miembros del equipo informados de los avances en tiempo real.
- **Productividad:** Reduce los cambios de contexto entre aplicaciones.
- **Colaboración eficiente:** Discute incidencias directamente en los canales de trabajo.

---

### **Caso de uso práctico**

Imagina un equipo que trabaja en el desarrollo de software:

1. Un desarrollador detecta un bug y crea un ticket en Jira desde Slack con `/jira create`.
2. El ticket se asigna automáticamente al equipo responsable, y todos los miembros reciben una notificación en el canal `#proyecto-backend`.
3. Un compañero comenta directamente en Slack sobre el ticket para aclarar detalles.
4. Una vez resuelto, Jira actualiza automáticamente el estado y notifica en Slack, informando al equipo del cierre de la incidencia.




# Referencias

- [Web oficial de Slack](https://slack.com/)
- [Planes de precios de Slack](https://app.slack.com/plans/T082GT9RAT0?geocode=es-es)
- [Primeros Pasos con Slack](https://slack.com/intl/es-es/help/articles/115004071768-%C2%BFQu%C3%A9-es-Slack#trabajar-en-slack)
- [Crear un nuevo espacio de trabajo con Slack](https://slack.com/intl/es-es/help/articles/206845317-C%C3%B3mo-crear-un-espacio-de-trabajo-de-Slack)


- [Guía de conexión de Jira con Slack](https://www.atlassian.com/es/software/jira/guides/integrations/tutorials#integrate-with-slack)
- [An easier way to use JIRA with Slack](https://slack.com/intl/es-es/blog/productivity/an-easier-way-to-use-jira-with-slack)
- [Guía de uso de Slack con Jira](https://www.atlassian.com/es/whitepapers/more-effective-teamwork-with-atlassian-and-slack)



<!--

Create an issue `/jira create <summary here>`

● Take action on issues in Slack by clicking the `...` menu to the right of the issue**Notifications**

Connect project

● Connect a project `/jira connect`

Personal notifications

● Get notified about your work `/jira notify`

Manage notifications

● Manage your notifications `/jira manage`

**Other**

Give feedback

● We'd love to hear what you think `/jira feedback`

Help menu

● View complete help menu `/jira help`

-->


