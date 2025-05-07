#### Description

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/483e50268fe7e015c49caf51a69063d0/capture.pcap). Recover the flag.



#### Hints
1. Try using a tool like Wireshark
2. What are streams?


#### Solucion
1. ```wget  https://jupiter.challenges.picoctf.org/static/483e50268fe7e015c49caf51a69063d0/capture.pcap```
2. ```Abrimos Wireshark
abrimos capture.pcap
buscamos algun UPD damos ctrl follow y UPD streams
buscamos de una en una y encontramos la bandera

picoCTF{StaT31355_636f6e6e}
```
