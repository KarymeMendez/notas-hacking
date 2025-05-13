#### Description

Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one? Image: [this](https://mercury.picoctf.net/static/b6205dd933ec01c022c4e6acbdf11116/dolls.jpg)

---
#### Hints
1. Wait, you can hide files inside files? But how do you find them?
2. Make sure to submit the flag as picoCTF{XXXXX}

---
#### Solucion

Le hicimos un exiftool para ver el contenido de imagen, desde el nombre,el tipo,despues le hicimos un binwalk para ver los archivos que estan incrustados que no vemos,nos sale que hay una imagen en base_images,buscamos que tiene la imagen 2_c_jpg le hacemos más binwalk y nos muestra más imagenes,repetimos el proceso y en la 4ta imagen, hay un archivo que se llama flag.txt solo le damos open flag.txt y nos muestra la bandera

 1. wget https://mercury.picoctf.net/static/1b70cffdd2f05427fff97d13c496963f/dolls.jpg              
2.  exiftool dolls.jpg                                                                
3. strings -n 10 dolls.jpg  
4. binwalk dolls.jpg
5. binwalk -e dolls.jpg
6. cd dolls.jpg.extracted
  7. cd base_images          
  8. open 2_c.jpg    
9. binwalk 2_c.jpg                  
10. binwalk -e 2_c.jpg 
11. cd _2_c.jpg.extracted/base_images
 12. open 3_c.jpg 
13. binwalk -e 3_c.jpg 
14. cd _3_c.jpg.extracted/base_images
15.  open 3_c.jpg       
16. binwalk -e 4_c.jpg 
17. cd _4_c.jpg.extracted/           
 18.  cat flag.txt
Tenemos la bandera --> picoCTF{bf6acf878dcbd752f4721e41b1b1b66b}                                                                                   