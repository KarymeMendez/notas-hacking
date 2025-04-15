
#### Description

Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/ende.py) using [this password](https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/pw.txt) to get [the flag](https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/flag.txt.en)?



##### Hints
1. Get the Python script accessible in your shell by entering the following command in the Terminal prompt: `$ wget https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/ende.py`
2. `$ man python`



#### Solucion
1. Descargar el archivo 
```
wget https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/ende.py
```
2. Descargar el archivo
```
wget https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/flag.txt.en
```
3. Escribimos en la terminal 
```
python ende.py -d flag.txt.en
```
Ingresamos la contraseña que esta en el archivo descargable
```
67c6cc9667c6cc9667c6cc9667c6cc96
```
Y nos da la bandera
```
picoCTF{4p0110_1n_7h3_h0us3_67c6cc96}
```