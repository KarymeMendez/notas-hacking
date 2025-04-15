
#### Description

Help us test the form by submiting the username as `test` and password as `test!`
Additional details will be available after launching your challenge instance.


#### Hints
1. any redirections?


#### Solucion

1. Entramos al link del sitio web que nos da picoCTF, nos logueamos con el usuario y la contraseña que previamente nos da al iniciar la instancia. Para ver como se comporta la pagina.
2. Regresamos al inicio de la pagina y la inspeccinamos, nos vamos al sitio de red y nos damos cuenta que en la ruta del link aparece un id con distintos valores al dar para atras o para adelante a la pagina. 
		Si damos hacia atrás será el id con el valor = **bF90aGVfd2F5X2JlNzE2ZDhlfQ==**
		Si damos hacia adelante será el id con el valor =  **cGljb0NURntwcm94aWVzX2Fs**

3. Si ambos valores los juntamos y lo pasamos a un DECODE BASE65 nos dara la bandera.

Unimos ambos id:
```
cGljb0NURntwcm94aWVzX2FsbF90aGVfd2F5X2JlNzE2ZDhlfQ==
```

Pasamos a un decode BASE65:
```
picoCTF{proxies_all_the_way_be716d8e}
```


