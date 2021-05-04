# PSQL

Entrar en postgres 

```
sudo su - postgres

psql
```

### Administrar 

> Acceder a la base de datos `psql "base de datos" "usuario"` 

> Salir de la terminal `\q`

> Ver las bases de datos que están creadas `\l`

> Crear bases de datos `CREATE DATABASE "database";`

> Mostrar tablas `\dt`

### Tablas



- Crear tabla con columnas 

```mysql
create table NOMBRETABLA(
  	id int,
  	nombre varchar,
 );
```



### Insert

```mysql
INSERT INTO nombre_tabla (columna1, columna2, columna3) VALUES (valor1, valor2, valor3);
```



### Transacción

 

```mysql
BEGIN;


UPDATE cuentas SET balance = balance - 137.00 WHERE nombre = 'Pepe';

UPDATE cuentas SET balance = balance + 137.00 WHERE nombre = 'Juan';

SELECT nombre, balance FROM cuentas WHERE nombre = 'Pepe' AND nombre = 'Juan';

COMMIT;	
```





### Rollback

