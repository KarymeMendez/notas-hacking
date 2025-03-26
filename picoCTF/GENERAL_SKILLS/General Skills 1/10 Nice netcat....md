There is a nice program that you can talk to by using this command in a shell: `$ nc mercury.picoctf.net 22342`, but it doesn't speak English...

Hints:

- You can practice using netcat with this picoGym problem: [what's a netcat?](https://play.picoctf.org/practice/challenge/34)
- You can practice reading and writing ASCII with this picoGym problem: [Let's Warm Up](https://play.picoctf.org/practice/challenge/22)

Solución 

```
karymeZapmen-picoctf@webshell:~$ nc mercury.picoctf.net 744
```

Después arrojara estos valores
```
112 105 99 111 67 84 70 123 103 48 48 100 95 107 49 116 116 121 33 95 110 49 99 51 95 107 49 116 116 121 33 95 102 50 100 55 99 97 102 97 125 10
```

Con ayuda podemos ver que son valores ASCII
```
112 -> p
105 -> i
99 -> c
111 -> o
67 -> C
84 -> T
70 -> F
123 -> {
103 -> g
48 -> 0
48 -> 0
100 -> d
95 -> _
107 -> k
49 -> 1
116 -> t
116 -> t
121 -> y
33 -> !
95 -> _
110 -> n
49 -> 1
99 -> c
51 -> 3
95 -> _
107 -> k
49 -> 1
116 -> t
116 -> t
121 -> y
33 -> !
95 -> _
102 -> f
50 -> 2
100 -> d
55 -> 7
99 -> c
97 -> a
102 -> f
97 -> a
125 -> }

```

Y al reemplazar numero por letra...
```
picoCTF{g00d_k1tty!_n1c3_k1tty!_f2d7cafa}

```