# PyDDoS
### Modern DDoS toolkit with Python3
* This is simple ddos script with python3 for education purpose.

### Methods:
| Method               |   Target   | Description |
| ---------------------| -----------|-------------|
| SMS                  | PHONE     | Sends a massive amount of SMS messages and calls to a single target |
| EMAIL                | EMAIL     | Sends a massive amount of Email messages to a target |
| NTP                  | IP:PORT    | NTP amplification is a type of Distributed Denial of Service (DDoS) attack in which the attacker exploits publically-accessible Network Time Protocol (NTP) servers to overwhelm the targeted with User Datagram Protocol (UDP) traffic. |
| SYN                  | IP:PORT    | A SYN flood (half-open attack) is a type of denial-of-service (DDoS) attack which aims to make a server unavailable to legitimate traffic by consuming all available server resources. |
| UDP                  | IP:PORT    | A UDP flood is a type of denial-of-service attack in which a large number of User Datagram Protocol (UDP) packets are sent to a targeted server with the aim of overwhelming that device’s ability to process and respond. The firewall protecting the targeted server can also become exhausted as a result of UDP flooding, resulting in a denial-of-service to legitimate traffic. |
| POD (Ping of Death)  | IP         | Ping of Death (a.k.a. PoD) is a type of Denial of Service (DoS) attack in which an attacker attempts to crash, destabilize, or freeze the targeted computer or service by sending malformed or oversized packets using a simple ping command. |
| ICMP                 | IP:PORT    | Ping flood, also known as ICMP flood, is a common Denial of Service (DoS) attack in which an attacker takes down a victim's computer by overwhelming it with ICMP echo requests, also known as pings. |
| HTTP                 | URL        | HTTP Flood is a type of Distributed Denial of Service (DDoS) attack in which the attacker manipulates HTTP and POST unwanted requests in order to attack a web server or application. These attacks often use interconnected computers that have been taken over with the aid of malware such as Trojan Horses. |
| Slowloris            | IP:PORT    | Slowloris is a denial-of-service attack program which allows an attacker to overwhelm a targeted server by opening and maintaining many simultaneous HTTP connections between the attacker and the target. |
| Memcached            | IP:PORT    | A memcached distributed denial-of-service (DDoS) attack is a type of cyber attack in which an attacker attempts to overload a targeted victim with internet traffic. The attacker spoofs requests to a vulnerable UDP memcached* server, which then floods a targeted victim with internet traffic, potentially overwhelming the victim’s resources. While the target’s internet infrastructure is overloaded, new requests cannot be processed and regular traffic is unable to access the internet resource, resulting in denial-of-service. |

### Installation:
* Windows:
  * Download Python 3 from here
  * Launch installer, click add python to PATH
  * Download PyDDoS
  * Open cmd or powershell in PyDDoS directory
  * Run this command: sudo pip install scapy
  * Run this command: pip install -r requirements.txt
  * And this: python pyddos.py --help
  
* Linux:
  * sudo apt update
  * sudo apt install python3 python3-pip git -y
  * git clone https://github.com/Anonymouz-cmd/PyDDoS.git
  * cd PyDDoS/
  * sudo pip install scapy
  * pip3 install -r requirements.txt
  * python3 pyddos.py --help

* Termux:
  * pkg update
  * pkg install python3 python3-pip git -y
  * git clone https://github.com/Anonymouz-cmd/PyDDoS.git
  * cd PyDDoS/
  * sudo pip install scapy
  * pip3 install -r requirements.txt
  * python3 pyddos.py --help

* Mac OS X
  * git clone https://github.com/Anonymouz-cmd/PyDDoS.git
  * cd PyDDoS/
  * sudo pip install scapy
  * pip install -r requirements.txt
  * python3 pyddos.py --help
 
### USAGE:
```
usage: pyddos.py [-h] [--target <IP:PORT, URL, PHONE>]
                 [--method <SMS/EMAIL/NTP/UDP/SYN/ICMP/POD/SLOWLORIS/MEMCACHED/HTTP>]
                 [--time <time>] [--threads <threads>]

Distributed Denial-of-Service Attack ToolKit

optional arguments:
  -h, --help            show this help message and exit
  --target <IP:PORT, URL, PHONE>
                        Target IP:port, url or phone
  --method <SMS/EMAIL/NTP/UDP/SYN/ICMP/POD/SLOWLORIS/MEMCACHED/HTTP>
                        Attack method
  --time <time>         time in secounds
  --threads <threads>   threads count (1-200)

For Example:
$ sudo python3 pyddos.py --method MEMCACHED --time 60 --threads 100 --target 127.0.0.1:80
$ python3 pyddos.py --method SMS --time 30 --threads 50 --target +66123456789
```
