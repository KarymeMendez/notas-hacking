
#### Description

The Rust saga continues? I ask you, can I borrow that, pleeeeeaaaasseeeee? Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/babfbee79718a6363826ba86300173ffde6d81577e9dd07d4130c53a7eecf6c3/fixme2.tar.gz).


#### Hints
1. https://doc.rust-lang.org/book/ch04-02-references-and-borrowing.html



#### Solucion
1. Descargamos el archivo
```
wget https://challenge-files.picoctf.net/c_verbal_sleep/3f0e13f541928f420d9c8c96b06d4dbf7b2fa18b15adbd457108e8c80a1f5883/fixme2.tar.gz
```

2. Ejecutamos el comando
```
cd fixme1
```

3. Ejecutamos el comando
```
cargo build
```
Nos da varios errores en el código.

4. Ejecutamos los comando
```
cd src

nano main.rs 
```
Corregimos errores de sintaxis, guardamos los cambios y salimos.

5. Volvemos a ejecutar 
```
cargo build

cargo run
```
Y nos da la bandera
```
picoCTF{4r3_y0u_h4v1n5_fun_y31?}
```