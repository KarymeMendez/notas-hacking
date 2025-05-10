#### Description

We found this [file](https://jupiter.challenges.picoctf.org/static/ab30fcb7d47364b4190a7d3d40edb551/mystery). Recover the flag.

---

#### Hints
1. Try fixing the file header

---

#### Solucion
	(Kali)
1. sudo wget https://jupiter.challenges.picoctf.org/static/ab30fcb7d47364b4190a7d3d40edb551/
2. file mystery       
3. exiftool mystery 
4. hexeditor mystery
5. hexeditor mystery
6. hexeditor mystery
7. hexeditor mystery
8. open mystery 

Tenemos la bandera
```
picoCTF{not_all_spaces_are_created_equal_3e2423081df9adab2a9d96afda4cfad6}
```