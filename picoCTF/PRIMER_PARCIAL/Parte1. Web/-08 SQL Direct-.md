#### Description

Connect to this PostgreSQL server and find the flag!
Additional details will be available after launching your challenge instance.


#### Hints
1. What does a SQL database contain?


#### Solucion
1. En kali Linux Ingresamos a lo que nos pide la descripcion
```
psql -h saturn.picoctf.net -p 60522 -U postgres pico

postgres
```
2. Ingresamos el comando "\dt"
```
Listado de relaciones
 Esquema | Nombre | Tipo  |  Dueño   
---------+--------+-------+----------
 public  | flags  | tabla | postgres
(1 fila)
```
3. Ingresamos el comando "select * from flags;"
```
id | firstname | lastname  |                address                 
----+-----------+-----------+----------------------------------------
  1 | Luke      | Skywalker | picoCTF{L3arN_S0m3_5qL_t0d4Y_73b0678f}
  2 | Leia      | Organa    | Alderaan
  3 | Han       | Solo      | Corellia
(3 filas)
```

Y nos da la bandera en la tabla anterior
```
picoCTF{L3arN_S0m3_5qL_t0d4Y_73b0678f}
```