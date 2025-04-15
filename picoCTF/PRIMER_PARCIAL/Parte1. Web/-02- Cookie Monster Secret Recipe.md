
#### Description
Cookie Monster has hidden his top-secret cookie recipe somewhere on his website. As an aspiring cookie detective, your mission is to uncover this delectable secret. Can you outsmart Cookie Monster and find the hidden recipe?You can access the Cookie Monster [here](http://verbal-sleep.picoctf.net:50164/) and good luck

#### Hints
1. Sometimes, the most important information is hidden in plain sight. Have you checked all parts of the webpage?
2. Cookies aren't just for eating - they're also used in web technologies!
3. Web browsers often have tools that can help you inspect various aspects of a webpage, including things you can't see directly.

#### Solucion
Al leer la descripcion del reto, sabremos que se trata de un reto web relacionado con **cookies HTTP** y **herramientas de desarrollo del navegador**.

1. Abrimos el sitio web
2. Inspeccionamos, nos vamos a la pestaña de **Aplicacion**, después en la sección de **Cookies** y analizamos el valor que nos lanza al momento de hacer log in en la pagina. El valor de la cookie es.
```
cGljb0NURntjMDBrMWVfbTBuc3Rlcl9sMHZlc19jMDBraWVzX0RFN0E1RTc2fQ%3D%3D
```
El valor parece estar codificado en **Base64**.

3. Nos pasamos a **CyberChef** para decodificarlo y... nos da la bandera.
```
picoCTF{c00k1e_m0nster_l0ves_c00kies_DE7A5E76}
```