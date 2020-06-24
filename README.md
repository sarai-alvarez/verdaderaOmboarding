
CÓMO CREAR UN MÓDULO DE BIBLIOTECA
Para crear un módulo de biblioteca en tu proyecto, haz lo siguiente:
1.	Haz clic en File > New > New Module.
2.	En la ventana Create New Module que aparece, haz clic en Android Library y, luego, en Next.
También se puede crear una biblioteca Java, que compila un archivo JAR tradicional. Si bien un archivo JAR es útil para muchos proyectos, en especial cuando deseas compartir el código con otras plataformas, no te permite incluir archivos de manifiesto ni recursos de Android, y esto es muy útil para reutilizar el código en proyectos de Android. Por ello, esta guía se enfoca en la creación de bibliotecas de Android.
3.	Otorga un nombre a la biblioteca y selecciona una versión mínima del SDK para el código de la biblioteca. Luego, haz clic en Finish.
Una vez que se haya completado la sincronización del proyecto de Gradle, se mostrará el módulo de la biblioteca en el panel Project de la izquierda. Si no se muestra la carpeta del módulo nuevo, asegúrate de que se muestre la vista Android.


ANATOMÍA DE UN ARCHIVO AAR
La extensión de un archivo AAR es .aar y el tipo de artefacto de Maven también debe ser aar. El archivo es de tipo zip y contiene las siguientes entradas obligatorias:
•	/AndroidManifest.xml
•	/classes.jar
•	/res/
•	/R.txt
•	/public.txt
Además, un archivo AAR puede incluir una o más de las siguientes entradas opcionales:
•	/assets/
•	/libs/name.jar
•	/jni/abi_name/name.so (donde abi_name es una de las ABI compatibles con Android)
•	/proguard.txt
•	/lint.jar
•	/api.jar









Desarrollo
Para el proyecto convertiremos en una librería un Omboarding, proyecto ya desarrollado en distintas ocasiones durante el semestre. Para ello hay una serie de pasos a seguir en base a los anteriores puntos.
Paso 1. Crer un nuevo proyecto
 
Paso 2.- Creamos el modulo 

A continuacion seleccionamos Android Library y presionamos en el boton Next.
 
Paso 4. Desarrollo del código.
La carpeta App es donde usualmente desarrollábamos nuestros códigos, en este caso como crearemos una librería no es necesario, dentro de esta carpeta APP no realizaremos nada.
Dentro de la carpeta mylibrary desarrollaremos el código del Omboarding, para ello creamos las carpetas necesarias, las clases necesarias, los layouts o estilos.

 
Paso 5.- Generamos el archivo AAR.
Nos ubicamos en Gradle y  damos doble clic en assemble para generar el archivo AAR.
 
Luego nos ubicaos en file y vamos a setings.
 
Buscas GitHub y ingresas tu usuario y contrasena, presionas en apply y luego en OK.
 



Paso 6
Ingresas a VCS , luego a import in to Version Control y presionas en Share Proyect on GitHub.
 
Definimos el nombre de la librería y presionamos en Share.
 
Paso 7. Dentro de nuestro GitHub seleccionamos el nombre de la librería
 
Presionamos en nueva versión y proporcionamos la versión .
 
Paso 8 ingresamos a la pagina Jitpack , dentro de su buscador ingresaremos el link de Github de nuestra librería.
 
 
Paso 9 creamos una nueva carpeta y ingresamos la dependencia que nos genero.
 
CAPTURAS
  [![INSERT YOUR GRAPHIC HERE](https://drive.google.com/file/d/10K1K6jv-ZpXEqEFLwYMVrmG2bzTC9aUw/view )]() 

CONCLUCIONES
Se realizó las investigaciones correspondientes  con lo cual se creó la librería en base al código desarrollado en el semestre, no obstante la librería no es  100% funcional puesto que no se logró hacer que  la información que se muestra dentro de cada una de las pantallas  sea editable.
