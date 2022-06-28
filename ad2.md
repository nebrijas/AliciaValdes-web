# Actividad dirigida 2

Este es el texto de la actividad dirigida 
En esta actividad dirigida 2, en primera instancia se procedió a realizar el cambio de **Readme.md** a la actividad dirigida 1 (**ad1.md**). En esta parte, no tuve ningún inconveniente, pero después surgieron algunas dudas y me quedé un poco en el proceso, como lo explicaré a continuación:

El desafío inició cuando había que convertir el archivo de Markdown a HTML. En este sentido, seguí estos pasos:
Accedo a https://github.com/nebrijas/AliciaValdes-web/settings/pages. Seguidamente en la pantalla, en branch, encontramos la opción **main** y y la opción **root**, la cual elegimos. Luego de activar estas opciones puede ver los cambios.
El siguiente paso que realicé fue dirigirme a Add file, y desde allí crear un nuevo archivo denominado ad2.md, documento en el que estoy escribiendo.
Después descargué GitBash y al abrirlo escribí **pwd** y presioné enter. Luego, escribí git clone, a la vez que colocaba el enlace https://github.com/nebrijas/AliciaValdes-web, cuyo objetivo era clonar la carpeta Git Hub a la computadora.
Para ver los resultados, presioné en **ls** y enter. 
Para acceder a ella, las indicaciones nos daba la opción de ultilizar **cd** junto al nombre de la carpeta. Luego volver a utilizar **ls** para visualizar el contenido que condensa dentro. 
En el siguiente paso es que descubrí que algunas cosas no salían del todo bien, pese a registrar mi nombre AliciaValdes-web, que en varias ocasiones se registró, seguía predominando **Desktop**, y al no saber cómo hacer cambios,  eso traía como consecuencia que algunas funciones no salieran como esperaba. Aunque pude culminar todo el proceso.
 
En esta misma línea de explicación. Continué con: `git config user.name`, seguido de mi nombre de usuario. Ejemplo: git config user.name AliciaValdes, enter.
En el siguiente paso escribí git config user.email, seguido del correo que utilizo en GitHub : alismontenegro822@h¿gmail.com. El resultados en estos dos últimos pasos no me convenció, puesto que no salió exactamente como debía salir, tras el ejemplo que mostró el profesor en clases. Así que esa es una de mis dudas y parte que debo reforzar en esta actividad.

Pese a estos inconvenientes, continué. Me dirigí al nageador de https://github.com/settings/tokens. 
Allí, le damos click a *generate new token* y le otorgamos el nombre en Note ( pd2). Elegimos la fecha de expiración, en este caso elegí 60 días. Continuando con esta confuguración en la opción de *select scopes*, tocamos en *repo*, mientras todas las demás opciones las obviamos. Finalmente **generamos token**.
Luego, regresé al progrma de Git bash, donde se escribe la palabra *echo* y en paréntesis el token. 

Acto seguido, escribí Readme.md ad1.md. Luego Readme.md. para copiar el contenido readme.m a ad1.md. Este proceso lo había realizado en github por lo que me aparecían los enlaces ad1.md y ad2.md. Le di a CTRL+X para salir ( tecla de control). 
Ya casi finalizando esta práctica, escribí **git status** para ver las modificaciones. 
Los últimos pasos consistieron en utilizar el git commit-m y por último git push, hasta allí llegué. 
