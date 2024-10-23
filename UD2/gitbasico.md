

# Uso básico de comandos Git

Git es un sistema de control de versiones distribuido (DVCS) desarrollado por el equipo de Linux. Es ampliamente utilizado por diversas plataformas de control de versiones, como GitHub, BitBucket y GitLab, para alojar proyectos de forma remota. Para interactuar con estos repositorios remotos desde nuestra máquina local, necesitamos instalar Git y usar sus diferentes comandos. Puedes encontrar una lista de los comandos más comunes de Git en la [chuleta de Git de GitHub](https://education.github.com/git-cheat-sheet-education.pdf). Este documento te guiará a través de la instalación de Git y el uso de algunos comandos básicos.

## 1. Instalación y Configuración de Git

La instalación de Git depende del sistema operativo.

* **Linux**: Para instalar Git, simplemente ejecuta el comando apropiado. Por ejemplo, en Ubuntu, utiliza:

    ```
    sudo apt-get install git
    ```

* **Windows y Mac**: Descarga la versión apropiada desde el [sitio web de Git](https://git-scm.com/downloads). En Mac, también puedes instalar Git instalando Xcode. En Windows

### 1.1. Configuración de Git

Antes de usar Git, es necesario configurar algunos ajustes predeterminados para conectarse a los servidores y almacenar credenciales. El comando `git config` se utiliza para establecer estas configuraciones en tres niveles:

* **Sistema**: Usando la opción `--system`, las configuraciones se aplican a todos los usuarios del sistema.
* **Usuario**: Con la opción `--global`, las configuraciones se aplican solo al usuario actual. Usaremos esta opción en esta sección.
* **Repositorio**: Específico para cada repositorio, permitiendo configuraciones únicas por proyecto.

Comienza estableciendo tu nombre completo con el siguiente comando (reemplaza *John Doe* con tu nombre real):

```
git config --global user.name "John Doe"
```

A continuación, configura el correo electrónico asociado con tu cuenta de GitHub:

```
git config --global user.email tuEmail@servidor.com
```

Opcionalmente, especifica un editor de texto predeterminado para Git. Esto es útil si Git necesita abrir un archivo de texto. Por ejemplo, en Windows, podrías usar:

```
git config --global core.editor notepad
```

Para evitar tener que escribir tus credenciales cada vez que te conectas a un repositorio, configura un ayudante de credenciales. Para GitHub, sigue [estas instrucciones](https://docs.github.com/es/get-started/getting-started-with-git/caching-your-github-credentials-in-git) para utilizar el **Git Credential Manager** recomendado, incluido por defecto con Git para Windows.

Ahora, Git está listo para usarse, incluso desde diferentes IDEs. Para ver la configuración actual, usa:

```
git config --list
```

Para comprobar la versión instalada de Git, usa:

```
git version
```

## 2. Comandos Básicos de Git Local

Aquí hay algunos comandos para trabajar con proyectos locales (sin conectarse a un repositorio remoto). Estos comandos son útiles tanto para proyectos locales como para proyectos remotos que se han descargado para trabajar sin conexión.

### 2.1. Creando un Repositorio Local

Para inicializar un nuevo repositorio local, primero crea la carpeta del proyecto y luego ejecuta:

```
git init
```

Esto inicializa la carpeta como un repositorio Git creando una subcarpeta oculta `.git` para la base de datos del repositorio. No necesitas preocuparte por esta subcarpeta.

Los archivos en el repositorio estarán en uno de tres estados: confirmado (committed), preparado (staged) o modificado (modified). Puedes cambiar los estados de los archivos usando varios comandos. Para verificar el estado del repositorio en cualquier momento, usa:

```
git status
```

> **Ejercicio 1:**
>
> Crea una carpeta llamada **GitEjercicios** en tu sistema. Dentro, crea una subcarpeta llamada **MiPrimerRepoLocal**, navega a esta carpeta y ejecuta `git init` para inicializarla como un repositorio Git.

### 2.2. Añadiendo o Editando Archivos

Después de agregar un nuevo archivo a la carpeta del repositorio (por ejemplo, *archivo.txt*), ejecuta `git status`. Git mostrará que hay archivos para añadir.



Para preparar los archivos, usa `git add`. Para un solo archivo:

```
git add archivo.txt
```

Para preparar todos los cambios a la vez, usa:

```
git add .
```

Repite el comando `git add` después de hacer cambios. Para deshacer la preparación de un archivo, usa:

```
git rm --cached archivo.txt
```

### 2.3. Confirmando Cambios (Commit)

Después de preparar los cambios, confírmalos en la base de datos del repositorio con:

```
git commit -m "Mi primer commit"
```

La opción `-m` te permite añadir un mensaje de confirmación, que es requerido para rastrear los cambios.

Alternativamente, usa `-a` para preparar y confirmar cambios en un solo paso:

```
git commit -a -m "Tu mensaje de commit"
```

**Visualizando el Historial de Commits**

Para ver el historial de commits, usa:

```
git log
```


Cada commit tiene una etiqueta única, que puede usarse para referenciar el commit más tarde.

**Visualizando Cambios**

Para ver los cambios entre versiones, usa:

* `git show`: Muestra los cambios en el último commit
* `git show cb1fd6f8`: Muestra los cambios en un commit específico
* `git diff`: Muestra los cambios aún no confirmados

> **Ejercicio 2:**
>
> Realiza los siguientes pasos en *MiPrimerRepoLocal*:
>
> - Crea un archivo llamado `archivo.txt` con el texto "Mi primer archivo de texto."
> - Prepara el archivo con `git add .`
> - Confirma los cambios con el mensaje "Mi primer commit"
> - Edita `archivo.txt` y añade una segunda línea con tu nombre
> - Prepara y confirma los cambios con `git commit -a -m "Mi segundo commit"`
> - Visualiza el historial de commits usando `git log`

**Etiquetando Commits**

Podemos añadir manualmente etiquetas a un commit dado, de modo que podamos encontrarlo fácilmente más tarde cuando queramos mostrar sus cambios. Usamos el comando `git tag`, seguido del nombre de la etiqueta:

```
git tag v1.0
```

Esto se aplica al último commit enviado. Luego, podemos mostrar los cambios de este commit con este comando:

```
git show v1.0
```

Si queremos etiquetar un commit que no es el último, entonces debemos especificar la etiqueta previa de este commit (o su prefijo inicial), después de la nueva etiqueta que queremos asignarle:

```
git tag v1.0 cb1fd6f8
```

### 2.4. Deshaciendo Cambios

Para volver a un commit previo, usa `git reset`:

```
git reset --hard 0305afd
```

Reemplaza *0305afd* con el prefijo de la etiqueta del commit.

**Nota adicional**

Si ya has publicado los cambios (por ejemplo, los has enviado a un repositorio remoto) y luego realizas un `git reset`, podrías encontrar problemas al intentar hacer push. Si es necesario, podrías forzar el push con:

```bash
git push --force
```

Pero ten mucho cuidado con esto, ya que otros usuarios pueden perder su trabajo si no se maneja adecuadamente.

### 2.5. El Archivo *.gitignore*

Añade un archivo `.gitignore` para especificar qué archivos o carpetas ignorar. Por ejemplo, para omitir todos los archivos `.exe`:

```
*.exe
```

Para omitir múltiples tipos de archivos o carpetas:

```
node_modules/
*.exe
*.tmp
```

> **Nota**: `.gitignore` no excluye archivos ya confirmados.

## 3. Trabajando con Repositorios Remotos

A continuación, veamos cómo conectarnos a un repositorio remoto de GitHub para subir/descargar cambios.

### 3.1. Clonando Repositorios

Para clonar un repositorio remoto, usa:

```
git clone https://github.com/usuario/nombre-del-repo
```

### 3.2. Actualizando Repositorios Locales

Para actualizar tu repositorio local con cambios del remoto, usa:

```
git pull
```

### 3.3. Enviando Cambios a Repositorios Remotos

Para subir cambios locales, sigue estos pasos:

1. Realiza cambios
2. Prepara los cambios con `git add .`
3. Confirma con `git commit`
4. Haz push con `git push`

> **Ejercicio 3:**
>
> Clona el repositorio *MiPrimerRepo*. Luego:
>
> 1. Añade un nuevo archivo llamado *lista_de_compras.txt*
> 2. Haz push del archivo al repositorio remoto
> 3. Verifica el archivo en GitHub
> 4. Clona el repositorio en otra carpeta
> 5. Añade un archivo llamado *tareas.txt* y haz push
> 6. Haz pull de los cambios desde la carpeta original de *MiPrimerRepo* para ver el archivo *tareas.txt*.

### 3.4. Añadiendo Repositorios Remotos

Puedes añadir un repositorio remoto a tu proyecto local usando el comando `git remote`. Esto es útil si has creado un repositorio local y ahora quieres subir tus cambios a una plataforma remota como GitHub o GitLab.

Primero, crea un repositorio en tu plataforma de alojamiento de Git (por ejemplo, GitHub) y copia la URL del repositorio.

En tu proyecto local, añade el repositorio remoto usando:

```
git remote add origin https://github.com/usuario/nombre-del-repo.git
```

Aquí, `origin` es el nombre del remoto (puedes elegir cualquier nombre, pero `origin` es la convención estándar).

Para verificar que el remoto ha sido añadido, ejecuta:

```
git remote -v
```

Esto mostrará las URLs del repositorio.

### 3.5. Enviando Cambios a Repositorios Remotos

Para subir cambios locales al repositorio remoto, sigue estos pasos:

1. Realiza cambios en los archivos de tu proyecto.
2. Prepara los cambios con:

    ```
    git add .
    ```

3. Confirma los cambios con un mensaje significativo:

    ```
    git commit -m "Mensaje de commit describiendo los cambios"
    ```

4. Envía los cambios al repositorio remoto. Si es la primera vez que haces push al repositorio y la rama en la que estás trabajando aún no existe en el repositorio remoto, necesitas establecer la rama upstream. Puedes hacerlo ejecutando:

    ```
    git push -u origin main
    ```

   La parte `main` se refiere a la rama a la que estás haciendo push, que típicamente es la rama predeterminada en la mayoría de los repositorios. Si tu rama tiene un nombre diferente, reemplaza `main` con el nombre correcto de la rama.

5. Después de establecer el upstream, los push posteriores pueden hacerse usando:

    ```sh
    git push
    ```

### 3.6. Actualizando Repositorios Locales

Para actualizar tu repositorio local con cambios del remoto, usa:

```sh
git pull origin main
```

o, si la rama upstream está establecida:

```sh
git pull
```

### 3.7. Enviando etiquetas a un repositorio remoto

1. **Crear una Etiqueta**: Puedes crear una etiqueta usando el siguiente comando. Puede ser una etiqueta anotada o ligera.

   - Para una etiqueta anotada (con un mensaje y metadatos):
     ```bash
     git tag -a v1.0 -m "Versión 1.0"
     ```

   - Para una etiqueta ligera (solo una etiqueta):
     ```bash
     git tag v1.0
     ```

2. **Enviar una Etiqueta Específica**: Si deseas enviar solo una etiqueta específica al repositorio remoto, utiliza el siguiente comando:

   ```bash
   git push origin v1.0
   ```

3. **Enviar Todas las Etiquetas**: Para enviar todas las etiquetas de una vez al repositorio remoto, utiliza el siguiente comando:

   ```bash
   git push --tags
   ```

   Esto enviará todas las etiquetas que has creado localmente y que aún no se han enviado al remoto.

4. **Verificar las Etiquetas en GitHub**: Puedes comprobar las etiquetas en tu repositorio en GitHub visitando la sección "Releases" o navegando a la pestaña "Tags".