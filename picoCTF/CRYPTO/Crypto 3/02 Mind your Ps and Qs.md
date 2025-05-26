#### Description

In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/b9ddda080c56fb421bf30409bec3460d/values)

---
#### Hints
1. Bits are expensive, I used only a little bit over 100 to save money
---
#### Solucion

1. Descargamos _values_
2. Le damos un cat a values, y nos da 3 variables 
```
c: 964354128913912393938480857590969826308054462950561875638492039363373779803642185
n: 1584586296183412107468474423529992275940096154074798537916936609523894209759157543
e: 65537
```
3. Entramos a FactorDB y factorizamos la n para que nos de dos valores p y q.
4. ponemos en la terminal de kali --> python. Colocamos lo siguiente
```
c = 964354128913912393938480857590969826308054462950561875638492039363373779803642185
>>> n = 1584586296183412107468474423529992275940096154074798537916936609523894209759157543
>>> e = 65537 
>>> p =  2434792384523484381583634042478415057961
>>> q = 650809615742055581459820253356987396346063
>>> p * q
1584586296183412107468474423529992275940096154074798537916936609523894209759157543
>>> tn = (p - 1) * (q - 1)
>>> 
>>> d = pow(e, -1, tn)
>>> 
>>> m = pow(c, d, n)
>>> 
>>> m
13016382529449106065927291425342535437996222135352905256639684640304028661985917
```

Para quitar la bandera en binario ponemos lo siguiente y damos enter --> >>> bytes.fromhex(hex(m)[2:]).decode()

Y nos da la bandera 
```
'picoCTF{sma11_N_n0_g0od_73918962}'
```
