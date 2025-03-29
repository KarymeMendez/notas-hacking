#### Description

Find the flag being held on this server to get ahead of the competition [http://mercury.picoctf.net:28916/](http://mercury.picoctf.net:28916/)

#### Hints 

1. Maybe you have more than 2 choices
2. Check out tools like Burpsuite to modify your requests and look at the responses


### Solución
en la pagina hay dos colores rojo y azul, uno nos manda get y otro post, entonces al checarlo con curl no muestra la llave, pero al mostrar HEAD que es el encabezado y ya por eso nos muestra la bandera.

Para saber la bandera hacemos lo siguiente:
```
HEAD http://mercury.picoctf.net:28916/
200 OK
Content-Type: text/html; charset=UTF-8
Client-Date: Sat, 29 Mar 2025 21:03:16 GMT
Client-Peer: 18.189.209.142:28916
Client-Response-Num: 1


Flag: picoCTF{r3j3ct_th3_du4l1ty_70bc61c4}
```