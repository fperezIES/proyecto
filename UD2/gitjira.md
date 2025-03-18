# Herramientas de Control de Versiones

## Integración de Git en Jira

Para integrar **Git** en **Jira** utilizando la versión gratuita, una opción común es hacerlo mediante la integración de **GitHub**. A continuación, se explica cómo realizar esta integración de manera sencilla.

### 1. **Integrar GitHub con Jira**

Puedes integrar **GitHub** con Jira utilizando la aplicación **GitHub for Jira**, disponible en el **Atlassian Marketplace**.

#### Pasos para integrar GitHub con Jira:

1. **Instalar la aplicación GitHub for Jira**:
    
    - En Jira, selecciona **Apps** en la barra de navegación superior y luego **Explorar más aplicaciones**.
        
    - Busca **GitHub for Jira** y selecciónala de los resultados.
        
    - Haz clic en **Obtener aplicación** y luego en **Consíguelo ahora**.
        
2. **Conectar una organización de GitHub**:
    
    - Después de instalar la aplicación, haz clic en **Empezar**. Si la aplicación ya está instalada, ve a **Apps** > **Administrar tus aplicaciones** y luego **GitHub for Jira**.
        
    - Haz clic en **Continuar**.
        
    - Selecciona **GitHub Cloud** y luego **Siguiente**.
        
    - Ingresa tu nombre de usuario y contraseña de GitHub, luego haz clic en **Iniciar sesión**.
        
    - Encuentra la organización que deseas conectar a Jira y haz clic en **Conectar**.
        
3. **Configurar los repositorios de GitHub**:
    
    - Durante la conexión, puedes elegir entre **Todos los repositorios** o **Solo repositorios seleccionados**.
        
    - Si seleccionas **Solo repositorios seleccionados**, elige los repositorios que deseas vincular a tu proyecto de Jira.
        

#### Uso de la integración:

- **Vinculación de actividades**: Puedes vincular **commits**, **pull requests** y **ramas** con issues de Jira escribiendo el número del issue en el mensaje del commit o en el nombre de la rama.
    
    - Por ejemplo, en un commit relacionado con un issue "PROY-456", al escribir el mensaje del commit debes comenzar escribiendo el identificador del issue. Ej: "PROY-456 Corregido problema de carga inicial de usuarios"
    - Si queremos asociar una rama al issue llamaremos a la rama con el identificador del issue.
#### Ventajas de la integración GitHub-Jira:

- **Visibilidad del código**: Jira muestra todos los commits y pull requests asociados a un issue.
    
- **Transiciones automáticas**: Puedes configurar que los issues en Jira cambien de estado cuando se realizan ciertos commits o se fusionan pull requests.
    
- **Reporte de código**: Jira ofrece informes sobre la actividad de los desarrolladores y el progreso del código vinculado a un proyecto.
    

### 2. **Visualización de Actividad de Git en Jira**

Una vez que hayas configurado la integración con GitHub, Jira mostrará automáticamente la actividad de Git vinculada a los issues. Podrás ver:

- **Commits**: Los commits asociados a un issue se mostrarán dentro del issue correspondiente en Jira.
    
- **Pull requests**: Se verán los pull requests relacionados con los issues, y se podrán revisar desde Jira.
    
- **Ramas**: Puedes ver qué ramas están asociadas a cada issue y su estado.
    

## Bibliografía

- [Integrar Jira con GitHub](https://support.atlassian.com/jira-cloud-administration/docs/integrate-jira-software-with-github/)
    
- [GitHub for Jira en Atlassian Marketplace](https://marketplace.atlassian.com/apps/1219592/github-for-jira?hosting=cloud&tab=overview)
    

Para complementar esta guía, puedes consultar el siguiente video que muestra cómo instalar la integración de GitHub para Jira Software desde la página de herramientas de Jira. Esta integración permite actualizaciones automáticas de los elementos de trabajo en Jira basadas en la actividad de GitHub.

<iframe width="560" height="315" src="https://www.youtube.com/embed/N-RZjp4og28?si=TzdrZ60cYRvzfKzC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>