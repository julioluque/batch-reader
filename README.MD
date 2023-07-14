# Spring Boot Batch

## POC - EJEMPLO BASE PREVIO A MIGRAR A VERSION 3

Usa la memoria para manipular los metadatos del proceso spring batch.

### Caracteristicas

- reader, lee de base de datos
- db to csv
- Java 8
- Spring 2
- Maven
- output logs en consola


### input

Tabla PERSONA de base de datos

### Model

```
CREATE TABLE persona(
id BIGINT AUTO_INCREMENT NOT NULL PRIMARY KEY,
nombre VARCHAR(30),
apellido VARCHAR(30),
direccion VARCHAR(30),
telefono VARCHAR(30)
);
```

### output

- resources/csv_output.csv

Ejemplo: 
```
nombre;apellido;direccion;+54 9 115telefono
Nombre 1;Apellido 1;Direccion 1;+54 9 1150000001
Nombre 2;Apellido 2;Direccion 2;+54 9 1150000002
Nombre 3;Apellido 3;Direccion 3;+54 9 1150000003
Nombre 4;Apellido 4;Direccion 4;+54 9 1150000004
Nombre 5;Apellido 5;Direccion 5;+54 9 1150000005
Nombre 6;Apellido 6;Direccion 6;+54 9 1150000006
Nombre 7;Apellido 7;Direccion 7;+54 9 1150000007
Nombre 8;Apellido 8;Direccion 8;+54 9 1150000008
Nombre 9;Apellido 9;Direccion 9;+54 9 1150000009
Nombre 10;Apellido 10;Direccion 10;+54 9 1150000010
Nombre 11;Apellido 11;Direccion 11;+54 9 1150000011
```

### Ejecutables

```
    mvn clean package
```

