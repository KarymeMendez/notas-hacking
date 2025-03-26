#### Description

My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/179/challenge.zip)

#### Hints 

1. `git branch -a` will let you see available branches
2. How can file 'diffs' be brought to the main branch? Don't forget to `git config`!
3. Merge conflicts can be tricky! Try a text editor like nano, emacs, or vim.

### Solucion

```
karymeZapmen-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/179/challenge.zip

karymeZapmen-picoctf@webshell:~$ unzip challenge.zip

karymeZapmen-picoctf@webshell:~$ cd drop-in

karymeZapmen-picoctf@webshell:~/drop-in$  git branch -a

karymeZapmen-picoctf@webshell:~/drop-in$ git checkout feature/part-1

karymeZapmen-picoctf@webshell:~/drop-in$ git log

karymeZapmen-picoctf@webshell:~/drop-in$cat flag.py

'PRIMERA PARTE DE LA BANDERA'

karymeZapmen-picoctf@webshell:~/drop-in$ git checkout feature/part-2

karymeZapmen-picoctf@webshell:~/drop-in$ git log

karymeZapmen-picoctf@webshell:~/drop-in$cat flag.py

'SEGUNDA PARTE DE LA BANDERA'

karymeZapmen-picoctf@webshell:~/drop-in$ git checkout feature/part-3

karymeZapmen-picoctf@webshell:~/drop-in$ git log

karymeZapmen-picoctf@webshell:~/drop-in$cat flag.py

'TERCERA Y ULTIMA PARTE DE LA BANDERA'


'LA COSTRUIMOS Y...'
picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_798f9981}
```