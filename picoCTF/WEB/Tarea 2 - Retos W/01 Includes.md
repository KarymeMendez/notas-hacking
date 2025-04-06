#### Description

Can you get the flag?

Additional details will be available after launching your challenge instance.

#### Hints 
1. Is there more code than what the inspector initially shows?


### Solucion
1. "Ctrl u" a la pagina que nos da la descripción del reto
2. Entramos a la hoja de estilos .css, nos muestra esto...
```
body {
  background-color: lightblue;
}

/*  picoCTF{1nclu51v17y_1of2_  */
```
Primera parte de la bandera.

3. Entramos a el archivo .js, nos muestra...
```
  
function greetings()
{
  alert("This code is in a separate file!");
}

//  f7w_2of2_6edef411}
```
Segunda parte de la bandera.


```
 picoCTF{1nclu51v17y_1of2_f7w_2of2_6edef411}
```