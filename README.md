# Análisis de Login con Java
El análisis de seguridad se realizara sobre el caso 2. https://www.studytonight.com/servlet/login-system-example-in-servlet.php

## Errores
Prevent SQL injection. Restringir las entradas, no permitir caracteres especiales, espacios en blanco, limite de caracteres.

No mantener las credenciales de la base de datos en el propio código. Extraer este contenido a un fichero de configuración y que esta información no se suba o guarde a ningún control de versiones.

Tener las contraseñas de los usuarios en base de datos en texto plano y realizar la comprobación de credenciales en la propia query. Lo correcto sería encriptar las contraseñas con una función hash y luego comprobar que la nueva contraseña equivale la encriptada  y guardada en base de datos. 

En el fichero html el campo de entrada para la contraseña es un campo de texto normal, lo que hace que la contraseña sea visible en todo momento.

## Herramientas:
 - IDE: Netbeans 8.2
 - Servidor: Glassfish 4.1.1
 - JDK: 1.8
 - DB: MySql 5.7 docker container

Se ha generado una Java Web Application con Netbeans y se han añadido los servlets correspondientes y las clases u otros
 ficheros necesarios.

Se ha desplegado mediante el servidor Glassfish 4.1.1 que viene integrado con la instalación de Netbeans.

Para la base de datos se ha utilizado le contenedor docker de 
MySql y mediante un script se han realizado las 
configuraciones necesarias para preparar la base de datos.
