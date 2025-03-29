#### Description

There is some interesting information hidden around this site [http://mercury.picoctf.net:39491/](http://mercury.picoctf.net:39491/). Can you find it?

#### Hints 
1. You should have enough hints to find the files, don't run a brute forcer.

### Solución
1. Ctrl u a la pagina y vemos una la primera parte ded la bandera "picoCTF{t".
2. en esa mismma ubicacion ingresamos a la hoja de estilos "mycss.css", y estara la segunda parte de la bandera "h4ts_4_l0".
3. nos regresamos al codigo inicial e ingresamos a archivo .js, en el dira una pista "How can I keep Google from indexing my website?" 
4. En el link proporcionado, al final colocamos robots.txt y encontramos la tercera parte de la bandera " t_0f_pl4c", pero tambien nos dice los siguiente _I think this is an apache server... can you Access the next flag?_.
5. quittamos "robots.txt" del link y ponemos ".htaccess" y nos dara la cuarta parte de la bandera "3s_2_lO0k" y dice _I love making websites on my Mac, I can Store a lot of information there._
6. quieamos ".htaccess" del link y ponemos ".DS_Store" y nos dara la ultima parte de la bandera "_f7ce8828}"

```
picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_f7ce8828}
```