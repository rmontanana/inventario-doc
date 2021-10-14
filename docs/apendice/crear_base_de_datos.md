##3.1.1 Crear una base de datos

Se puede crear una base de datos a través de utilidades como [MySQL Workbench](http://dev.mysql.com/downloads/workbench/ "Descargar Workbench") o bien a través del cliente MySQL de la línea de comandos.

Para conectarse con el servidor MySQL tecleamos el siguiente comando desde el terminal

    mysql -u root -p

Al pulsar _intro_ se nos pedirá la contraseña del usuario root en MySQL. No tiene por qué ser el usuario _root_, vale con cualquier usuario de MySQL que tenga derechos para crear bases de datos.

Una vez dentro del programa tecleamos:

    create database Inventario character set utf8 collate utf8_general_ci;
    grant all on Inventario.* to prueba identified by 'pruebas123';

Con el primer comando creamos una base de datos llamada <code>Inventario</code> con el conjunto de caracteres [utf8](http://es.wikipedia.org/wiki/UTF-8) para los datos almacenados. El segundo comando concede todos los derechos sobre la base de datos _Inventario_ al usuario <code>prueba</code> (si no existía este usuario se crea en este momento) y se le asigna la contraseña <code>pruebas123</code>
