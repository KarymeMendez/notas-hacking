#### Description
Welcome to the challenge! In this challenge, you will explore a web application and find an endpoint that exposes a file containing a hidden flag.The application is a simple blog website where you can read articles about various topics, including an article about API Documentation. Your goal is to explore the application and find the endpoint that generates files holding the server’s memory, where a secret flag is hidden.

Additional details will be available after launching your challenge instance.


### Hints
1. Explore backend development with us
2. The head was dumped.


### Solucion

1. Lanzamos la instancia e ingresamos al link
2. Ingresamos a la documentación de API e indagamos, nos damos cuenta que hay en la seccion de **Diagnosing** hay un GET y enseguida el nombre del reto, ingresamos ahi.
3. Nos damos cuenta que hay un archivo descargable donde podria estra la bandera, ingresamos y en el se encuentran al parecer muchisimos datos sobre nodos, buscamos coincidencias con la palabra "pico" y encontramos la banera.

```
picoCTF{Pat!3nt_15_Th3_K3y_bed6b6b8}
```