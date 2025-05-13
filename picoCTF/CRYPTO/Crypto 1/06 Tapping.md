#### Description

Theres tapping coming in from the wires. What's it saying `nc jupiter.challenges.picoctf.org 48247`.

---
#### Hints
1. What kind of encoding uses dashes and dots?
2. The flag is in the format PICOCTF{}

---
#### Solucion
1. Entramos al servidor que nos pide, nos da un codigo morse --> .--. .. -.-. --- -.-. - ..-. { -- ----- .-. ... ...-- -.-. ----- -.. ...-- .---- ... ..-. ..- -. .---- ..--- -.... .---- ....- ...-- ---.. .---- ---.. .---- } 
2. Lo pasamos al cyberchef y obtenemos la bandera
	--> PICOCTF{M0RS3C0D31SFUN1261438181}