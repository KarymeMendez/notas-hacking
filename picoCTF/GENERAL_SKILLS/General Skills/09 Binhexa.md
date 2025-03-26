#### Description

How well can you perfom basic binary operations?

Additional details will be available after launching your challenge instance.


### Hints
(None)


### Solucion

```
karymeZapmen-picoctf@webshell:~$ nc titan.picoctf.net 49631

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 10100100
Binary Number 2: 11000000


Question 1/6:
Operation 1: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 10000000
Correct!

Question 2/6:
Operation 2: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 01100000
Correct!

Question 3/6:
Operation 3: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 111101100000000
Correct!

Question 4/6:
Operation 4: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11100100
Correct!

Question 5/6:
Operation 5: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 101100100
Correct!

Question 6/6:
Operation 6: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 101001000
Correct!

Enter the results of the last operation in hexadecimal: 0x148

Correct answer!


The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_6ab1ad84}
```


#### Referencias
https://es.planetcalc.com/911/#google_vignette

