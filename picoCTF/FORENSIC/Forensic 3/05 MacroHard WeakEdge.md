#### Description

I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/d3dd8cd51524d9fafcccd1b7d55f85e7/Forensics is fun.pptm)

---
#### Hints
1. None

---
#### Solucion
1. wget https://mercury.picoctf.net/static/d3dd8cd51524d9fafcccd1b7d55f85e7/Forensics%20is%20fun.pptm
2. file Forensics\ is\ fun.pptm
3. unzip Forensics\ is\ fun.pptm
4. echo "Z m x h Z z o g c G l j b 0 N U R n t E M W R f d V 9 r b j B 3 X 3 B w d H N f c l 9 6 M X A 1 f Q" | tr -d " " | base64 -d

Tenemos la bandera ---> picoCTF{D1d_u_kn0w_ppts_r_z1p5}
