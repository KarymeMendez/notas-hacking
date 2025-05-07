#### Description

This is a really weird text file [TXT](https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt)? Can you find the flag?



#### Hints
1. How do operating systems know what kind of file it is? (It's not just the ending!
2. Make sure to submit the flag as picoCTF{XXXXX}


#### Solucion
1. ```get https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt```

2. ```file flag.txt.1```
3. ```mv flag.txt.1 flag.png```
4. ```open flag.png```



Tenemos la bandera --> picoCTF{now_you_know_about_extensions}