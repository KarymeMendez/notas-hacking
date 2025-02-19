#### Description

Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `481e7b14`

Additional details will be available after launching your challenge instance.


#### Hints
1. Finding a cheatsheet for bash would be really helpful!


## Solución

```
karymeZapmen-picoctf@webshell:~$ ssh ctf-player@venus.picoctf.net -p 53189

ctf-player@pico-chall$ cat 1of3.flag.txt

ctf-player@pico-chall$ cat 2of3.flag.txt

ctf-player@pico-chall$ cd ~

ctf-player@pico-chall$ cat 3of3.flag.txt

```


#### Respuesta
```
picoCTF{xxsh_0ut_0f_\/\/4t3r_1118a9a4}
```