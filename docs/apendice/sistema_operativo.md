##3.2 Utilidades
La aplicación necesita de dos utilidades para poder realizar las copias de seguridad de la aplicación: <code>mysqldump</code> y <code>gzip</code>.

La primera es una utilidad de MySQL y se necesita para hacer un volcado de toda la información almacenada en la base de datos, la segunda es una utilidad del sistema operativo y permite comprimir el archivo de copia de seguridad de la base de datos y las imágenes asociadas.

En la opción de configuración hay dos casillas en las que se especifica a la aplicación dónde están ubicadas ambas en el servidor. Si la opción de copia de seguridad falla, habrá que revisar la configuración para poner los datos correctos. Para averiguar esta información hay que teclear en una sesión de terminal del servidor los siguientes comandos:

    which mysqldump
    which gzip

Para cada uno de los comandos aparecerá una información que tendremos que copiar en las casillas correspondientes de la pantalla de configuración.
