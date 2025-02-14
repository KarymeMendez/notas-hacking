#### Description
Can you convert the number 42 (base 10) to binary (base 2)?

Solucion.
En python...
```
 print(bin(42)[2:])
```

- bin(42) convierte el número 42 a su representación binaria en Python, pero incluye un prefijo `0b` que indica que es un número binario.
- Usar `[2:]` eliminamos los dos primeros caracteres (`0b`) para obtener solo la parte binaria.

Respuesta. 101010



