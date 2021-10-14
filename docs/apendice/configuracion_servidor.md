##3.1.2 Configuración servidor
Hay que asegurarse de que el charset con el que trabaja el servidor MySQL es utf8 para poder comprobarlo podemos utilizar el cliente de la línea de comandos o utilidades como [MySQL Workbench](http://dev.mysql.com/downloads/workbench/ "Descargar Workbench") eso se entra en mysql y mediante el comando status se averigua. Se puede cambiar en my.cnf o mediante workbench crear/modificar el fichero de configuración.
Contenido mínimo del fichero /etc/my.cnf

    [mysqld]
    character-set-server = utf8
    collation-server = utf8_spanish_ci

    [client]
    default-character-set=utf8
