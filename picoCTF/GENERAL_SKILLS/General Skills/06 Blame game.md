#### Description

Someone's commits seems to be preventing the program from working. Who is it?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/159/challenge.zip)
#### Hints 
1. In collaborative projects, many users can make many changes. How can you see the changes within one file?
2. Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).
3. You can use `python3 <file>.py` to try running the code, though you won't need to for this challenge.



### Solucion
```
karymeZapmen-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/159/challenge.zip

karymeZapmen-picoctf@webshell:~$ unzip challenge.zip

karymeZapmen-picoctf@webshell:~$ cd drop-in

karymeZapmen-picoctf@webshell:~$ git log message.py


picoCTF{@sk_th3_1nt3rn_81e716ff}
```