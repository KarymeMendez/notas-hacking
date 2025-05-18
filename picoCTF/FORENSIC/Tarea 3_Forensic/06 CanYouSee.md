#### Description
How about some hide and seek? Download this file [here](https://artifacts.picoctf.net/c_titan/131/unknown.zip).

---
#### Hints
1. How can you view the information about the picture?
2. If something isn't in the expected form, maybe it deserves attention?

---
#### Solucion
1. Descargamos -->  wget https://artifacts.picoctf.net/c_titan/131/unknown.zip
2. unzip unknown.zip
3. exiftool ukn_reality.jpg
4. echo cGljb0NURntNRTc0RDQ3QV9ISUREM05fZDhjMzgxZmR9Cg== | base64 -d
Obtenemos la bandera --> ``` picoCTF{ME74D47A_HIDD3N_d8c381fd}```