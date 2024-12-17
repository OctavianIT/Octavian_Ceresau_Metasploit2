# **Metasploit pt - 2**
## **net discover**
```bash
fping -a -g 192.168.1.0/24
```
​➡️ [Risultato](https://github.com/OctavianIT/Octavian_Ceresau_Metasploit2/blob/main/Octavian_Ceresau_Metasploit2/0.png)

## **nmap**
Scansiono i servizi attivi sulla macchina target
```bash
nmap -sV -T5 192.168.1.40
```
➡️ [Risultato](https://github.com/OctavianIT/Octavian_Ceresau_Metasploit2/blob/main/Octavian_Ceresau_Metasploit2/1.png)

## **framework**
Avvio framework
```bash
msfconsole
```
## **modulo**
scegliamo questo modulo perchè vogliamo attaccare la porta 23 "telnet"
```bash
search type:auxiliary telnet
```
➡️[Modulo](https://github.com/OctavianIT/Octavian_Ceresau_Metasploit2/blob/main/Octavian_Ceresau_Metasploit2/3.png)

## **utilizzo modulo**
```bash
use auxiliary/scanner/telnet/telnet_version
```
## **configurazione**
```bash
set threads 4
set rhosts 192.168.1.40
```

## **avvio modulo**
```bash
exploit
```
➡️[Avvio](https://github.com/OctavianIT/Octavian_Ceresau_Metasploit2/blob/main/Octavian_Ceresau_Metasploit2/6.png)


