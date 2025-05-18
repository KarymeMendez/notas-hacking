#### Description
I've gotten bored of handing out flags as text. Wouldn't it be cool if they were an image instead? You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_atlas/14/challenge.zip)

The same files are accessible via SSH here: `ssh -p 51600 ctf-player@atlas.picoctf.net` Using the password `84b12bae`. Accept the fingerprint with `yes`, and `ls` once connected to begin. Remember, in a shell, passwords are hidden!

---
#### Hints
1. QR codes are a way of encoding data. While they're most known for storing URLs, they can store other things too.
2. Mobile phones have included native QR code scanners in their cameras since version 8 (Oreo) and iOS 11
3. If you don't have access to a phone, you can also use zbar-tools to convert an image to text
---
#### Solucion
1. Descragamos -->wget https://artifacts.picoctf.net/c_atlas/16/challenge.zip
2. unzip challenge.zip
3. cd home/ctf-player/drop-in/
4. open flag.png
Nos abre una imagen con un codigo QR, lo escanemos con el celular y nos da la bandera.
```
picoCTF{p33k_@_b00_0194a007}
```