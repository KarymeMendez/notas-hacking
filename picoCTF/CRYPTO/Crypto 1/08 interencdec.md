#### Description
Can you get the real meaning from this file. Download the file [here](https://artifacts.picoctf.net/c_titan/1/enc_flag).

---
#### Hints
1. Engaging in various decoding processes is of utmost importance

---
#### Solucion
1. wget https://artifacts.picoctf.net/c_titan/1/enc_flag
2. cat enc_flag 
3. cat enc_flag | base64 -d
4. echo d3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrX2xoNjBsMDBpfQ== | base64 -d
Nos da como salida --> wpjvJAM{jhlzhy_k3jy9wa3k_lh60l00i}

Lo pasamos a cyberchef con ROT13 con 19 vueltas y obtenemos la bandera --> picoCTF{caesar_d3cr9pt3d_ea60e00b}

