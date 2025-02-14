#### Description

What does this `bDNhcm5fdGgzX3IwcDM1` mean? I think it has something to do with bases.

## Solucion 1
```
>>> import base64
>>> import base64
>>> encoded = "bDNhcm5fdGgzX3IwcDM1"
>>> decoded = base64.b64decode(encoded).decode('utf-8')
>>> print(decoded)
```

- `base64.b64decode()` decodifica el texto de base64 a su forma binaria original.
- `.decode('utf-8')` convierte los bytes decodificados en una cadena de texto.

Respuesta. l3arn_th3_r0p35


