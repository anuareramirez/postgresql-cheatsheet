# postgresql-cheatsheet

#Ingresar a postgresql
```
username# psql
```

#Salir de postgresql
```
database# \q
```

#Ayuda
```
username# psql --help
database# \?
database# help
```

#Conectarse a una base de datos
```
username# psql nombredebasededatos -h localhost -p 5432 -U anuareramirez
database# \c nombredebasededatos
```

#Crear base de datos
```
database# CREATE DATABASE nombredebasededatos;
```

#Listar base de datos
```
database# \l
```

#Eliminar base de datos
```
database# DROP DATABASE nombredebasededatos;
```

#Crear nueva tabla
```
database# CREATE TABLE nombredetabla (
  columna1 tipo constrains,
  ... );
```
  
#Listar tablas
```
database# \d
database# \dt
```

#Listar campos de tabla
```
database# \d nombredetabla
```

#Eliminar tabla
```
database# DROP TABLE nombredetabla;
```

#Crear un registro en tabla


#Crear registro desde archivo sql
```
database# \i ruta/al/archivo/con/terminacion.sql
```

#Listar contenido de tabla
```
database# SELECT * FROM nombredetabla;
```

#Listar contenido de tabla con columnas personalizadas
```
database# SELECT columnaX, ... FROM nombredetabla;
```

#Listar contenido de tabla con orden ascendente columna personalizada
```
database# SELECT * FROM nombredetabla ORDER BY columnaX ASC;
```

#Listar contenido de tabla con orden descendente columna personalizada
```
database# SELECT * FROM nombredetabla ORDER BY columnaX DESC;
```

#Listar contenido de tabla con orden descendente columna personalizada
```
database# SELECT * FROM nombredetabla ORDER BY columnaX DESC;
```

#Listar contenido de tabla con columna personalizada y resultados unicos
```
database# SELECT DISTICT columnaX FROM nombredetabla ORDER BY columnaX;
```

#Listar contenido de tabla con filtros WHERE, AND y OR
```
database# SELECT * FROM nombredetabla WHERE columnaX = 'string1' AND (columnaY = 'string2' OR columnaY = 'string3');
```






