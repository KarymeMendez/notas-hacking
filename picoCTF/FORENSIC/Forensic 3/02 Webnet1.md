#### Description

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/picopico.key). Recover the flag.

---
#### Hints
1. Try using a tool like Wireshark.
2. How can you decrypt the TLS stream?

---
#### Solucion
1. Descargamos --> wget https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/capture.pcap
2. Descargamos --> wget https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/picopico.key
3. Comando --> file capture.pcap.3
4. Comando --> wireshark capture.pcap.3  
5. Comando --> strings  vulture.jpg -n15
	Obtenemos la bandera --> picoCTF{honey.roasted.peanuts}





