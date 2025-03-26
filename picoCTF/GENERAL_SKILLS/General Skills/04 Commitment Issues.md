
Description 
I accidentally wrote the flag down. Good thing I deleted it! You download the challenge files here: challenge.zip

#### Hints 
1. Version control can help you recover files if you change or lose them!
2. Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control)
3. You can 'checkout' commits to see the files inside them

### Solución

```
wget https://artifacts.picoctf.net/c_titan/76/challenge.zip

unzip challenge.zip

karymeZapmen-picoctf@webshell:~$ cd drop-in

karymeZapmen-picoctf@webshell:~/drop-in$ ls -a

$ git log

git checkout e720dc26a1a55405fbdf4d338d465335c439fb3e

	HEAD is now at e720dc2 create flag

$ cat message.txt

	picoCTF{s@n1t1z3_ea83ff2a}
```