#### Description

Download this disk image and find the flag. Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/137/disk.flag.img.gz)

---
Hints
1. None

---
Solucion
1. Descargamos imagen
2. descomprimimos
3. fls nombre_imagen -o 360448
4. fls nombre_imagen -o 360448 -r  | grep flag
5. icat  imagen -o 360448 2371 

nos da la bandera --> ```picoCTF{by73_5urf3r_adac6cb4}```