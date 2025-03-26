
#### Description

What was I last working on? I remember writing a note to help me remember...You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/66/challenge.zip)


#### Hints 
1. The `cat` command will let you read a file, but that won't help you here!
2. Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).
3. When committing a file with git, a message can (and should) be included.

### Solución

```
karymeZapmen-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/66/challenge.zip

karymeZapmen-picoctf@webshell:~$ unzip challenge.zip

karymeZapmen-picoctf@webshell:~$ cd drop-in

karymeZapmen-picoctf@webshell:~/drop-in$ git init .

karymeZapmen-picoctf@webshell:~/drop-in$ cat message.txt

karymeZapmen-picoctf@webshell:~/drop-in$ cd .git

karymeZapmen-picoctf@webshell:~/drop-in/.git$ cat COMMIT_EDITMSG

picoCTF{t1m3m@ch1n3_d3161c0f}
```

