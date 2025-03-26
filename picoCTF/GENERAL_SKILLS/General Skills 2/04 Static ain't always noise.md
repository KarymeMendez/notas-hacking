#### Description

Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/ec4dbd8898ade34e1d60d5b70c1b8c8c/static)? This [BASH script](https://mercury.picoctf.net/static/ec4dbd8898ade34e1d60d5b70c1b8c8c/ltdis.sh) might help!

#### Solucion

```
wget https://mercury.picoctf.net/static/ec4dbd8898ade34e1d60d5b70c1b8c8c/static

wget https://mercury.picoctf.net/static/ec4dbd8898ade34e1d60d5b70c1b8c8c/ltdis.sh

chmod +x static

cat static.ltdis.strings.txt

cat static.ltdis.strings.txt | grep pico

```

##### Respuesta
picoCTF{d15a5m_t34s3r_98d35619}


