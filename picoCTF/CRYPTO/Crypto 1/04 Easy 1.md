#### Description
The one time pad can be cryptographically secure, but not when you know the key. Can you solve this? We've given you the encrypted flag, key, and a table to help `UFJKXQZQUNB` with the key of `SOLVECRYPTO`. Can you use this [table](https://jupiter.challenges.picoctf.org/static/1fd21547c154c678d2dab145c29f1d79/table.txt) to solve it?.

---
#### Hints
1. Submit your answer in our flag format. For example, if your answer was 'hello', you would submit 'picoCTF{HELLO}' as the flag.
2. Please use all caps for the message.
---
#### Solucion
1. Descargamos el archivo (table.txt)
2. Pasamos a cyberchef, pegamos la llave y la bandera encriptada y lo decodificamos con vigenere
	Obtenemos  la bandera ---> picoctf{CRYPTOISFUN}