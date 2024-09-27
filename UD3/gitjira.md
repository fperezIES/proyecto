
# Integración de Git en Jira

Para integrar **Git** en **Jira** utilizando la versión gratuita, la forma más común es hacerlo mediante la integración de **Bitbucket**, otro producto de Atlassian, o **GitHub** si usas esa plataforma para gestionar repositorios de código. A continuación, te explico cómo hacer ambas integraciones de manera sencilla.

### 1. **Integrar Bitbucket con Jira (Recomendado)**

Bitbucket es el servicio de repositorios Git de Atlassian, por lo que la integración entre **Jira** y **Bitbucket** es muy fluida y está completamente disponible en la versión gratuita de Jira.

#### Pasos para integrar Bitbucket en Jira:

1. **Crea una cuenta en Bitbucket** (si aún no tienes una):
    
    - Ve a [bitbucket.org](https://bitbucket.org/) y regístrate con el mismo correo electrónico que usas para Jira.
2. **Vincular Bitbucket con Jira**:
    
    - Inicia sesión en tu cuenta de **Jira**.
    - Ve a la configuración del proyecto que quieres vincular a Bitbucket.
    - En el menú lateral, selecciona "**Integrations**" o "**Integraciones**".
    - En la sección de integraciones, busca la opción de **Bitbucket** y haz clic en "**Conectar**".
    - Sigue las instrucciones para autenticarte en tu cuenta de Bitbucket y autoriza la conexión entre ambos servicios.
3. **Crear un repositorio de Bitbucket**:
    
    - Una vez conectado, puedes crear un repositorio nuevo en Bitbucket o seleccionar uno existente que quieras vincular a tu proyecto en Jira.
    - Después de crear el repositorio, todas las actividades relacionadas con los commits, pull requests y ramas que se vinculen a un issue de Jira aparecerán en el tablero de Jira.

#### Uso de la integración:

- Puedes enlazar **commits**, **pull requests** y **branches** (ramas) a **issues de Jira** agregando el número del issue en el mensaje del commit o el nombre de la rama. Por ejemplo:
    - Si estás trabajando en un issue con el código "PROY-123", puedes crear una rama llamada `PROY-123-implementar-autenticacion`.
    - Luego, cuando realices un commit o crees un pull request, Jira lo enlazará automáticamente con ese issue.

#### Ventajas de la integración Bitbucket-Jira:

- **Seguimiento de código**: Puedes ver en Jira todos los commits, ramas y pull requests relacionados con un issue.
- **Transición automática**: Puedes configurar reglas para que los issues cambien de estado automáticamente en Jira cuando se creen pull requests o se hagan commits (ejemplo: pasar un issue de "En progreso" a "En revisión").
- **Visualización**: Puedes ver directamente en Jira el estado del código sin necesidad de cambiar de herramienta.

---

### 2. **Integrar GitHub con Jira**

Si prefieres usar **GitHub** en lugar de Bitbucket, también puedes integrarlo con Jira fácilmente utilizando un **Power-Up gratuito** llamado **GitHub for Jira**.

#### Pasos para integrar GitHub con Jira:

1. **Crea una cuenta en GitHub** (si no tienes una):
    
    - Ve a [github.com](https://github.com) y regístrate.
2. **Instalar la integración GitHub for Jira**:
    
    - Ve a **Atlassian Marketplace** (o desde Jira, dirígete a la sección de Power-Ups o "Apps").
    - Busca **GitHub for Jira** e instálalo.
    - Durante el proceso de instalación, se te pedirá autenticarte con tu cuenta de GitHub.
3. **Conectar repositorios de GitHub**:
    
    - Una vez instalado el Power-Up, conecta tu cuenta de GitHub a Jira.
    - Selecciona los repositorios que deseas vincular a tu proyecto de Jira.

#### Uso de la integración:

- Al igual que con Bitbucket, puedes vincular **commits**, **pull requests** y **branches** con issues de Jira escribiendo el número del issue en el mensaje del commit o el nombre de la rama.
- Por ejemplo, en un commit relacionado con un issue "PROY-456", puedes escribir un mensaje como `Fix authentication issue [PROY-456]`, y Jira lo enlazará automáticamente al issue correspondiente.

#### Ventajas de la integración GitHub-Jira:

- **Visibilidad del código**: Jira muestra todos los commits y pull requests asociados a un issue.
- **Transiciones automáticas**: Puedes configurar que los issues en Jira cambien de estado cuando se hacen ciertos commits o se fusionan pull requests.
- **Reporte de código**: Jira ofrece informes sobre la actividad de los desarrolladores y el progreso del código vinculado a un proyecto.

---

### 3. **Visualización de Actividad de Git en Jira**

Una vez que hayas configurado cualquiera de las integraciones (Bitbucket o GitHub), Jira mostrará automáticamente la actividad de Git vinculada a los issues. Podrás ver:

- **Commits**: Los commits asociados a un issue se mostrarán dentro del issue correspondiente en Jira.
- **Pull requests**: Se verán los pull requests relacionados con los issues, y se podrán revisar desde Jira.
- **Ramas**: Puedes ver qué ramas están asociadas a cada issue y su estado.

---

### Conclusión

Tanto **Bitbucket** como **GitHub** se integran fácilmente con **Jira** en la versión gratuita, permitiendo una sincronización fluida entre el código y la gestión de proyectos. La integración te permitirá realizar un seguimiento del desarrollo del software directamente desde Jira, agilizando el flujo de trabajo y asegurando que cada issue esté correctamente asociado al código que se está trabajando.

Esta integración es especialmente útil en proyectos colaborativos, ya que proporciona a los desarrolladores y gestores de proyectos visibilidad completa sobre el progreso y la calidad del código en tiempo real.