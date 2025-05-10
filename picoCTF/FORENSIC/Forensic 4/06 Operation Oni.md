#### Description

Download this disk image, find the key and log into the remote machine. Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

Additional details will be available after launching your challenge instance.

---
Hints
1. None

---
Soluicion
1. descargamos imagen
2. descomprimimos imagen
3. ls -lah imagen
4. mmls imagen
5. fls imagen -o 206848
6. fls imagen -o 206848 470
7. fls imagen -o 206848 3916
8. icat imagen -o 206848 2345 > key_file
9. file key_file
10. `ssh -i key_file -p 55446 ctf-player@saturn.picoctf.net`
Tenemos la bandera -->  