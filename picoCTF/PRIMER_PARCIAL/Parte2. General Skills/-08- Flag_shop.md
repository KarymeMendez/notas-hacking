
#### Description

There's a flag shop selling stuff, can you buy a flag? [Source](https://jupiter.challenges.picoctf.org/static/64e724ad327f83ad833d9c6baa072b1f/store.c). Connect with `nc jupiter.challenges.picoctf.org 4906`.


#### Hints
1. Two's compliment can do some weird things when numbers get really big!



#### Solución
Al parecer simula una tienda de banderas donde puedes ver el saldo, comprar banderas o salir.
Pero el chiste esta en que el sistema tiene un **saldo limitado** que se maneja como un número entero. Si introduces un número grande que el sistema no puede manejar correctamente, el **overflow** (desbordamiento) puede ocurrir, causando que el valor del saldo cambie de forma inesperada (por ejemplo, se convierte en un valor mucho mayor).

Entonces solo queda interactuar con el sistema hasta encontrar la bandera.
```
picoCTF{m0n3y_bag5_9c5fac9b}
```