#### Description

We found this [file](https://mercury.picoctf.net/static/d0129ad98ba9258ab59e7700a1b18c14/tunn3l_v1s10n). Recover the flag.

---
#### Hints
1. Weird that it won't display right...

---
#### Solucion
1. wget https://mercury.picoctf.net/static/21c07c9dd20cd9f2459a0ae75d99af6e/tunn3l_v1s10n
2. file tunn3l_v1s10n 
3. xxs tunn3l_v1s10n | head
4. xxd tunn3l_v1s10n | head
5. hexeditor tunn3l_v1s10n.bmp
6. mv tunn3l_v1s10n tunn3l_v1s10n.bmp 
7. open tunn3l_v1s10n.bmp 
	Obtenemos la bandera ---> picoCTF{qu1t3_a_v13w_2020}



