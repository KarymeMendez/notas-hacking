
#### Description

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key). Recover the flag.

---
#### Hints
1. Try using a tool like Wireshark.
2. How can you decrypt the TLS stream?

---
#### Solucion
1. Descargamos --> wget https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap
2. Descargamos --> wget https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key
3. Comando --> file capture.pcap.1 
4. Comando --> wireshark capture.pcap.2 
	Obtenemos la bandera --> picoCTF{nongshim.shrimp.crackers}

