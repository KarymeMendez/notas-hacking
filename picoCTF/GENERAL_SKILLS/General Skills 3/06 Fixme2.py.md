#### Description

Fix the syntax error in the Python script to print the flag.[Download Python script](https://artifacts.picoctf.net/c/4/fixme2.py)


#### Hints
1. Are equality and assignment the same symbol?
2. To view the file in the webshell, do: `$ nano fixme2.py`
3. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
4. The `str_xor` function does not need to be reverse engineered for this challenge.


### Solucion
```
wget https://artifacts.picoctf.net/c/4/fixme2.py

nano fixme2.py
```
CORREGIMOS ERRORES DE SINTAXIS, GUARDAMOS Y EJECUTAMOS
```
python3 fixme2.py
That is correct! Here's your flag:

picoCTF{3qu4l1ty_n0t_4551gnm3nt_e8814d03}
```