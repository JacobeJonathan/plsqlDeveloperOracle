# plsqlDeveloperOracle
-- creando un usuario
CREATE USER nombre_de_usuario IDENTIFIED BY contraseña;

select * from libros as ventas where id_libro between '3' and '5'
-- Insert in to target tables
-- First create the tables
create table top_salescustomers(prod_id int , cust_id int, time_id int , cust_first_name varchar(50), cust_last_name varchar(50), amount_sold varchar(50))
insert into top_salescustomers
values (1,1,1,'cola','real','23')

select * from top_salescustomers
-- contando la tabla
SELECT COUNT(*) FROM nombre_de_la_tabla;
-----------------------------------
select sysdate from dual
-- utilizando between
SELECT * FROM ventas WHERE fecha BETWEEN '2022-01-01' AND '2022-12-31';

-- creando tablas
create table maestro_materiales(
cd_mat int,
description varchar2(50),
fecha_creacion date,
peso number(10,3),
estado char(1)
)

select * from maestro_materiales
-- alteramos la tabla
alter table maestro_materiales
-- modificamos nombre de la tabla
rename to maestro_mate
-- agregar columna  una tabla
alter table maestro_mate
add fecha_creacion date
-- insertar
inner join maestro_mate( cd_mat, descripcion, fecha_creacion)
values(1,'hola','11-05-2023')
