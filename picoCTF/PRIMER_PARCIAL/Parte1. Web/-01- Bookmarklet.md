#### Description
Why search for the flag when I can make a bookmarklet to print it for me?
Additional details will be available after launching your challenge instance.

### Hints
1. A bookmarklet is a bookmark that runs JavaScript instead of loading a webpage.
2. What happens when you click a bookmarklet?
3. Web browsers have other ways to run JavaScript too.

#### Solucion
1. Ingresamos al sitio web que se genera al lanzar la instancia
2. Analizamos la pagina principal y observamos que nos da un codigo.
```
javascript:(function() { var encryptedFlag = "àÒÆÞ¦È¬ëÙ£ÖÓÚåÛÑ¢ÕÓÉÕËÆÒÇÚËí"; var key = "picoctf"; var decryptedFlag = ""; for (var i = 0; i < encryptedFlag.length; i++) { decryptedFlag += String.fromCharCode((encryptedFlag.charCodeAt(i) - key.charCodeAt(i % key.length) + 256) % 256); } alert(decryptedFlag); })();
```
3. Lo pasamos a la IA para que nos ayude a entenderlo un poco, tambien lo podemos ejecutar en la consola que aparece al inspeccionar la pagina, al generarlo nos da la banera.
```
var encryptedFlag = "àÒÆÞ¦È¬ëÙ£Ö�ÓÚåÛÑ¢ÕÓÉÕËÆÒÇÚËí";
var key = "picoctf";
var decryptedFlag = "";

for (var i = 0; i < encryptedFlag.length; i++) {
    decryptedFlag += String.fromCharCode(
        (encryptedFlag.charCodeAt(i) - key.charCodeAt(i % key.length) + 256) % 256
    );
}

console.log(decryptedFlag);



VM895:11 picoCTF{p@g3_turn3r_cebccdfe}
```