#### Description

Download this disk image and find the flag. Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/213/disk.flag.img.gz)

---
Hints
1. None

---
Solucion
1. descargamso imagen
2. fls imagen -o 411648
3. fls imagen -o 411648 472
4. openssl aes -salt -d -in imagen -out flag.txt -k  unbrea
5. cat flag.txt
Nos da la bandera --->   ```picoCTF{h4un71ng_p457_5113beab}```
