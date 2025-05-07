#### Description

Find the flag in this [picture](https://jupiter.challenges.picoctf.org/static/916b07b4c87062c165ace1d3d31ef655/pico_img.png).


#### Hints
1. What does meta mean in the context of files?
2. Ever heard of metadata?



#### Solucion
1. wget https://jupiter.challenges.picoctf.org/static/916b07b4c87062c165ace1d3d31ef655/pico_img.png
2. exiftool pico_img.png 
3. Nos da la bandera --> picoCTF{s0_m3ta_d8944929}