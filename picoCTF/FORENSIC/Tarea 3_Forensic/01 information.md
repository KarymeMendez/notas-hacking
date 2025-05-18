
#### Description
Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/b4d62f6e431dc8e563309ea8c33a06b3/cat.jpg)

---
#### Hints
1. Look at the details of the file
2. Make sure to submit the flag as picoCTF{XXXXX}
---
#### Solucion
1. Descargamos --> wget https://mercury.picoctf.net/static/d1375e383810d8d957c04eef9e345732/cat.jpg

2. file cat.jpg  
3. exiftool cat.jpg
En la license parece algo encriptado, entonces lo paso a cyberchef me da la opcion de que parece base 64, lo decodifica y sale la bandera.
```
picoCTF{the_m3tadata_1s_modified}
```