# DevOps

## ¿Qué es DevOps?

El término DevOps proviene de la combinación de los términos "development" (desarrollo) y "operations" (operaciones), y promueve la coordinación y colaboración de estos dos equipos para ofrecer productos de mejor calidad, más confiables y de forma más rápida. De esta manera, se pone fin al aislamiento entre los equipos de desarrollo y operaciones.

Al adoptar DevOps se adopta un conjunto de prácticas, herramientas y filosofía que permite automatizar e integrar procesos que comparten los equipos de desarrollo y de operaciones.


## Fases del ciclo de vida en DevOps

En el marco de trabajo DevOps el equipo de desarrollo y de operaciones de TI colaboran durante todo el ciclo de vida de un producto. 

En DevOps el ciclo de vida no es un proceso lineal con un final, sino que cada fase es contínua y se retroalimenta del resto de fases. Por ello, se utiliza un bucle infinito para representar esas fases y cómo se relacionan entre sí. Este bucle representa la necesidad de mejora y colaboración constante en cada iteración a lo largo de todo el ciclo de vida del producto.
 
<p align="center">
  <img src="devopsJ.png">
</p>

En DevOps se pueden identificar las siguientes fases:

1. **Planificación**: En esta fase se definen los objetivos, requisitos y tareas del proyecto a partir de los requisitos proporcionados por el cliente. En esta fase se utilizan herramientas de gestión de proyectos para organizar y priorizar las tareas. Algunas de las más utilizadas son Jira y Trello.

2. **Codificación**: el equipo de desarrollo se encarga de escribir el código e integrarlo en un repositorio compartido. En esta fase es necesario utilizar herramientas que permitan almacenar, compartir y llevar un control de versiones de todo el código. Algunas herramientas utilizadas son GitHub y GitLab.
   
3. **Construcción**: En esta fase el código se compila para poder ser ejecutado y se construyen los artefactos necesarios para la compilación. Aquí se incluye la automatización de la construcción del software para asegurar la consistencia y eficiencia en diferentes plataformas y entornos de despligue (pruebas, preproducción, producción...). Algunas herramientas utilizadas en esta fase son Docker, Ansible, Puppet o JFrog ARtifactory. Estas herramientas nos permiten gestionar versiones y compilaciones. 

4. **Pruebas**: Una vez construido el código se realizan pruebas automatizadas y manuales para asegurar que el software funciona de forma correcta y cumple con los requisitos necesarios. Las pruebas continuas ayudan a identificar y corregir errores de forma rápida. Herramientas como JUnit, Selenium o Codeception permiten programar estas pruebas.

5. **Liberación (Release)**: En esta fase se construye una versión del software que se entregará al usuario final. Para ello, habrá que asegurarse de que el software esté listo para ser utilizado en producción.

6. **Despliegue o Implementación**: El software se despliega en el entorno de producción. La implementación continua permite que los cambios se entreguen rápidamente y con menos riesgo.

7. **Operaciones**: Se centra en asegurar que los entornos de ejecución están correctamente dimensionados y configurados para que se garantice el funcionamiento correcto del software. Los entornos de ejecución que se utilizan normalmente son:
   - Entorno de desarrollo: la máquina de cada miembro del equipo.
   - Entrono de pruebas: donde se ejecuta la última versión del software disponible.
   - Entrono de pre-producción: intenta replicar el entorno de producción tanto como se pueda: misma versión y actualizaciones del SO, misma configuración de hardware, última versión del software etc.
   - Entorno de producción: entorno donde los usuarios tendrán acceso al software.
   
8. **Monitorización y Retroalimentación**: Se recopilan datos y comentarios de los usuarios y del sistema para identificar áreas de mejora. Esta información se utiliza para planificar futuras actualizaciones y mejoras, realimentando de esta manera la fase de planificación. Algunas herramientas que se pueden utilizar para ello son Grafana y Prometheus, herramientas que nos permiten obtener medidas sobre el rendimiento del sistema, incluyendo uso de la memoria y CPU, tráfico de red, tiempos de respuesta etc. 

## Las 7Cs de DevOps
Las fases del ciclo de vida en DevOps se agrupan en lo que se conoce como las 7Cs, que se encargan de guiar el proceso de desarrollo de software de principio a fin y de una forma contínua: desarrollo contínuo (CD), intengración contínua (CI), pruebas contínuas, despliegue contínuo, retroalimentación contínua, monitorización contínua y operaciones contínuas

1. **Desarrolo contínuo (CD)**: esta fase implica la planificación y codificación del software. DevOps fomenta lanzamientos de software regulares y frecuentes. Para ello, cada vez que se crea un trozo de código, se prueba, se construye y se despliega en producción. De esta manera, se mejora la calidad del código y se agiliza la detección y correción de fallos.
   
2. **Integración contínua (CI)**: cuando el desarrollador finaliza una parte del código en su máquina, lo integra en el repositorio compartido. Una vez allí se construye una versión de la apliación y se pasa la batería de pruebas, lo que ayuda a detectar errores rápidamente.
   
3. **Pruebas contínuas**: las pruebas se automatizan para garantizar que cada cambio de código sea seguro y funcione adecuadamente.

4. **Despliegue contínuo**: consiste en el proceso de desplegar la aplicación de forma automática en el entorno de producción cuando se hayan completado las fases de pruebas y constucción.
   
5. **Retroalimentación contínua**: una vez los usuarios utilizan la aplicación nos pueden enviar comentarios sobre el redimiento, fallos detectados o cualquier otra cosa que afecte a la experiencia del usuario. Gracias a esta retroalimentación continua se mejora el rendimiento de la aplicación y se reducen los fallos en el código.
    
6. **Monitorización contínua**: consiste en la supervisión constante de las aplicaciones y de la infraestructura que las aloja para detectar y resolver problemas rápidamente.
   
7. **Operaciones contínuas**: las operaciones continuas tienen como objetivo minimizar el tiempo de inactividad y evitar interrupciones en el servicio a los usuarios. Se intenta optimizar las aplicaciones y entornos para obtener una mayor estabilidad y rendimiento. También contribuye a alimentar la fase de planificación mediante informes de errores y mejoras planteadas por los usuarios.


---

### Debate:

¿En qué fases crees que interviene un desarrollador y cómo?
¿Y un administrador de sistemas?


### Vídeo
En el siguiente <a href="https://www.youtube.com/watch?v=_I94-tJlovg">video</a> puedes ver una explicación sencilla de en qué consiste DevOps. 


