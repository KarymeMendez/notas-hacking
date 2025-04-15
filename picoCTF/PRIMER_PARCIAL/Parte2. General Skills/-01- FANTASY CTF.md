
#### Description

Play this short game to get familiar with terminal applications and some of the most important rules in scope for picoCTF. Connect to the program with netcat: `$ nc verbal-sleep.picoctf.net 63159`



#### Hints
1. When a choice is presented like [a/b/c], choose one, for example: `c` and then press Enter.



#### Solucion
1. Entrar a la terminal y conectarnos
```
`$ nc verbal-sleep.picoctf.net 63159`
```
2. Dar enter cada que lo pida para continuar
3. Poner opcion a en lo siguiente
```
Options:
A) *Register multiple accounts*
B) *Share an account with a friend*
C) *Register a single, private account*
[a/b/c] > a


Options:
A) *Play the game*
B) *Search the Ether for the flag*
[a/b] > a
```
Seguir dando enter hasta que aparezca la bandera...

```
picoCTF{m1113n1um_3d1710n_76b680a5}
```