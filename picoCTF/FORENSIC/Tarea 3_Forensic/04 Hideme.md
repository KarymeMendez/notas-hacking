#### Description
Every file gets a flag. The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](https://artifacts.picoctf.net/c/259/flag.png).

---
#### Hints
1. None

---
#### Solucion
1. Descragamos --> ```wget https://artifacts.picoctf.net/c/257/flag.png```
2. ```file flag.png```
3. ```zsteg flag.png ```
4. ```exiftool flag.png ```
5. binwalk -e flag.png
6. cd _flag.png.extracted
7. cd secret
8. open flag.png
Obtenemos la bandera --> ``` picoCTF{Hiddinng_An_imag3_within_@n_ima9e_cda72af0}```
