1. ¿Qué ventaja tiene registrar las dependencias del proyecto en
requirements.txt en lugar de compartir la carpeta .venv?
La principal ventaja es que requirements.txt guarda solo la lista 
de librerías y sus versiones, mientras que .venv contiene todo el 
entorno virtual instalado, que puede ser muy pesado y depender del 
sistema operativo.

2. ¿Cómo identificaste el comando necesario cuando la práctica no lo 
proporcionó?
Consultando la documentación de Git y buscando el comando según la 
acción que necesitaba realizar.

3. ¿Qué diferencia existe entre preparar un archivo para un commit y 
crear el commit?
Prepararlo lo coloca en el área de preparación; crear el commit 
registra definitivamente esos cambios en el historial.

4. ¿Cómo puedes comprobar en qué rama estás trabajando?
Con el comando git branch.

5. ¿Cómo puedes determinar qué archivos fueron modificados antes de 
registrarlos?
Con el comando git status.

6. ¿Cómo puedes observar exactamente qué cambió dentro de un archivo?
Con el comando git diff.

7. ¿Por qué debe reconstruirse .venv después de obtener un repositorio?
Porque normalmente .venv no se comparte y cada usuario debe crear su 
propio entorno virtual.

8. ¿Qué relación existe entre requirements.txt y .gitignore?
.gitignore evita subir .venv, mientras que requirements.txt guarda las 
dependencias necesarias para reconstruirlo.

9. ¿Por qué la colaboración se realiza desde una rama y no 
directamente desde main?
Para trabajar sin afectar directamente la versión principal del 
proyecto y poder revisar los cambios antes de integrarlos.

10. ¿Por qué una solicitud de cambios no requiere crear un Pull 
Request nuevo?
Porque los nuevos commits realizados en la misma rama actualizan 
automáticamente el Pull Request existente.

11. Después de realizar el merge en GitHub, ¿por qué todavía es 
necesario actualizar el repositorio local?
Porque el merge ocurre en el repositorio remoto y la copia local debe 
descargar esos cambios con git pull. 

¿Qué diferencia existe entre preparar un archivo para un commit y crear el commit?Preparar (git add) selecciona qué cambios irán al área de preparación (staging area); crear el commit (git commit) guarda de forma permanente esos cambios preparados en el historial del repositorio.
¿Cómo puedes comprobar en qué rama estás trabajando?
Con el comando git branch (la rama activa aparece marcada con un *) o mediante git status.  
 ¿Cómo puedes determinar qué archivos fueron modificados antes de registrarlos?
Con el comando git status.   
¿Cómo puedes observar exactamente qué cambió dentro de un archivo?Con el comando git diff (o git diff --staged para cambios ya preparados).
¿Por qué debe reconstruirse .venv después de obtener un repositorio?
Porque .venv no se sube al repositorio al contener binarios, librerías y rutas absolutas específicas del sistema operativo del desarrollador original.  
 ¿Qué relación existe entre requirements.txt y .gitignore?
requirements.txt especifica las dependencias necesarias y sus versiones para el proyecto, mientras que .gitignore evita que la carpeta .venv (donde se instalan esas dependencias) se suba al repositorio.  
 ¿Por qué la colaboración se realiza desde una rama y no directamente desde main?
Para mantener la estabilidad del proyecto en producción (main), permitiendo probar y desarrollar cambios de forma aislada sin interrumpir a otros colaboradores.   
¿Por qué una solicitud de cambios no requiere crear un Pull Request nuevo?
Porque el Pull Request está vinculado a la rama origen; al hacer nuevos commits y un git push en esa misma rama, la solicitud existente se actualiza automáticamente.   Después de realizar el merge en GitHub,
 ¿por qué todavía es necesario actualizar el repositorio local?
Porque el merge integra los cambios únicamente en el servidor de GitHub; es necesario hacer git pull origin main localmente para descargar e integrar esas modificaciones en la copia de tu equipo.