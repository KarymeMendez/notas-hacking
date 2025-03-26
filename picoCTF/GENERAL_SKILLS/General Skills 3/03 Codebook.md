#### Description

Run the Python script `code.py` in the same directory as `codebook.txt`.
- [Download code.py](https://artifacts.picoctf.net/c/2/code.py)
- [Download codebook.txt](https://artifacts.picoctf.net/c/2/codebook.txt)

#### Hints
1. On the webshell, use `ls` to see if both files are in the directory you are in
2. The `str_xor` function does not need to be reverse engineered for this challenge.


```
wget https://artifacts.picoctf.net/c/2/code.py

wget https://artifacts.picoctf.net/c/2/codebook.txt

python3 code.py

picoCTF{c0d3b00k_455157_7d102d7a}
```
