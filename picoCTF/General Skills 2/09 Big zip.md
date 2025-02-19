#### Description

Unzip this archive and find the flag.

- [Download zip file](https://artifacts.picoctf.net/c/504/big-zip-files.zip)

## Hints
Can grep be instructed to look at every file in a directory and its subdirectories?

#### Solución
```
wget https://artifacts.picoctf.net/c/504/big-zip-files.zip

unzip big-zip-files.zip

grep -R picoCTF{

```


#### Respuesta
```
picoCTF{gr3p_15_m4g1c_ef8790dc}
```
