#### Description

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/13/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/13/level2.flag.txt.enc) in the same directory too.


### Hints
1. Does that encoding look familiar?
2. The `str_xor` function does not need to be reverse engineered for this challenge.


### Solucion

```
wget https://artifacts.picoctf.net/c/13/level2.py
wget https://artifacts.picoctf.net/c/13/level2.flag.t
xt.enc

karymeZapmen-picoctf@webshell:~$  nano level2.py
```
ANALIZAMOS EL CODIGO Y ENTENDEMOS QUE HAY UNA CADENA QUE ES UNA CONCATENACION DE LOS CARACTERES REPESENTADOS POR LOS VALORES HEXADECIMALES `0x64`, `0x65`, `0x37` y `0x36`. SI LOS COLOCAMOS EN CYBERCHEF EQUIVALE A "de76" que seria la contraseña
```
karymeZapmen-picoctf@webshell:~$  python3 level2.py
Please enter correct password for flag: de76

Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_489dea9a}
```