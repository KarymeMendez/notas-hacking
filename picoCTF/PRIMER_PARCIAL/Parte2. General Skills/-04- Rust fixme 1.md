
#### Description

Have you heard of Rust? Fix the syntax errors in this Rust file to print the flag! Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/3f0e13f541928f420d9c8c96b06d4dbf7b2fa18b15adbd457108e8c80a1f5883/fixme1.tar.gz).



#### Hints
1. Cargo is Rust's package manager and will make your life easier. See the getting started page [here](https://doc.rust-lang.org/book/ch01-03-hello-cargo.html)
2. [println!](https://doc.rust-lang.org/std/macro.println.html)
3. Rust has some pretty great compiler error messages. Read them maybe?


#### Solucion
1. Descargamos el archivo
```
wget https://challenge-files.picoctf.net/c_verbal_sleep/3f0e13f541928f420d9c8c96b06d4dbf7b2fa18b15adbd457108e8c80a1f5883/fixme1.tar.gz
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
picoCTF{4r3_y0u_4_ru$t4c30n_n0w?}
```