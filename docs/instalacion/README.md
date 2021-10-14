# 1. Instalación
Para instalar la aplicación basta con seguir estos pasos:
###0. Descargar los archivos de la aplicación
Hay que descargar el paquete con los archivos correspondientes preferiblemente de la última versión estable de:

<http://bitbucket.org/rmontanana/inventario2/downloads>
###1. Copiar los archivos en una ubicación a la que tenga acceso el usuario con el que se ejecuta el servidor Apache (apache, _www, etc.).

    mkdir Inventario
    cd Inventario
    unizp ../1.02.zip
    o
    tar xvzf ../1.02.tgz

###2. Crear un directorio temporal y dar derechos de escritura a los ficheros de configuración.
    mkdir tmp
    mkdir img.data
    chown apache tmp img.data
    chown apache inc/configuracion.inc
    chown apache inc
###3. Crear una base de datos en MySQL con el siguiente comando
    create database Inventario character set utf8 collate utf8_spanish_ci;
###4. Dar todos los derechos de acceso a esa base de datos a un usuario:
    grant all on Inventario.* to usuario identified by "contraseña";
###5. Conectarse a la aplicación en la url donde se ha instalado:
    http://<url>
Al hacer esto se arrancará automáticamente el programa de instalación con el que terminaremos de configurar la aplicación.

