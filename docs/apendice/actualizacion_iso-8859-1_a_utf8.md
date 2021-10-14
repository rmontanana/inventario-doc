##3.1.3 Conversión iso-8859-1 a utf8

Para actualizar una base de datos que haya sido creada con el conjunto de caracteres iso-8859-1, tan sólo hay que modificar el tipo de la base de datos y de las tablas a utf8 mediante workbench o mediante los siguientes comandos:

    use Inventario2;
    alter database Inventario2 character set utf8 collate utf8_spanish_ci;
    alter table Articulos convert to character set utf8 collate utf8_spanish_ci;
    alter table Ubicaciones convert to character set utf8 collate utf8_spanish_ci;
    alter table Elementos convert to character set utf8 collate utf8_spanish_ci;
    alter table Usuarios convert to character set utf8 collate utf8_spanish_ci;
