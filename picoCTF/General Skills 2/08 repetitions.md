#### Description

Can you make sense of this file?Download the file [here](https://artifacts.picoctf.net/c/475/enc_flag).


#### Hints
1. Multiple decoding is always good.


#### Solución
```
 wget https://artifacts.picoctf.net/c/475/enc_flag

cat enc_flag

karymeZapmen-picoctf@webshell:~$ cat enc_flag | base64 -d | base64 -d | base64 -d | base64 -d | base64 -d | base64 -d
```


#### Respuesta
```
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_492767d2}
```

