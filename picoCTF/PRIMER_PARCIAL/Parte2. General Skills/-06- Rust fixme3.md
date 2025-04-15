
#### Description

Have you heard of Rust? Fix the syntax errors in this Rust file to print the flag! Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/dcdaf491b35c1d0f5075e9583edbbb7aaea1dffb6ad32bc000e4d87b5200ff7b/fixme3.tar.gz).


#### Hints
1. Read the comments...darn it!


#### Solucion
1. Descargamos el archivo
```
wget https://challenge-files.picoctf.net/c_verbal_sleep/3f0e13f541928f420d9c8c96b06d4dbf7b2fa18b15adbd457108e8c80a1f5883/fixme3.tar.gz
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
picoCTF{n0w_y0uv3_f1x3d_1h3m_411}
```