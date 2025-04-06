#### Description

The flag is somewhere on this web application not necessarily on the website. Find it.

Additional details will be available after launching your challenge instance.

#### Hints 
1. (None)


#### Solucion
1. Entramos a la url y tambien le escribimos "/robots.txt". Recibimos esto...
```
User-agent *
Disallow: /cgi-bin/
Think you have seen your flag or want to keep looking.

ZmxhZzEudHh0;anMvbXlmaW
anMvbXlmaWxlLnR4dA==
svssshjweuiwl;oiho.bsvdaslejg
Disallow: /wp-admin/
```

2. Lo colocamos en cyberchef y nos da...
```
flag1.txtjs/myfif§2ö×fÆRçG@
```
3. Borramos "/robots.txt" y ponemos "/js/myfile.txt" para tener la banera
```
picoCTF{Who_D03sN7_L1k5_90B0T5_718c9043}
```