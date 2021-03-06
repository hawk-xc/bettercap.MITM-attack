# bettercap.MITM-attack
Man In The Middle attack practice
lebih tepatnya kita meracuni ARP atau Address Resolution Protocol pada jaringan korban. dimana informasi yang berasal dari korban akan diredirect ke komputer Attacker terlebih dahulu sebelum menuju URL tujuan. disini kita akan menggunakan tools Bettercap.

saya menggunakan OS Kali linux. tools ini opsional nya sudah terinstall default. jika menggunakan selain Kali linux install dengan perintah. `sudo apt-get install bettercap`

### COMMAND TO RUN
RUN bettercap tools `sudo bettercap` <br>
#### table command http protocol (no SSL)
| command | information |
|---------|-------------|
| help | to show bettercap option |
| help (option) | to shown specific option information |
| net.probe on | start the net.probe to scan all live host in network |
| help arp.spoof | show information about arp.spoof |
| set arp.spoof.internal true | enable arp.spoof module |
| set arp.spoof.targets (target ip) | spoof victim arp |
| arp.spoof on | enable arp spoof |
| set net.sniff.output (directory to save capt file) | for enable /home/user/Document/pentest.pcap |
| net.sniff on | enable net sniff |

#### table command https protocol (with SSL)
| command | information |
|---------|-------------|
| help https.proxy | shown specific information about https.proxy |
| set https.proxy.sslstrip true | enable https.proxy mode (true) |
| set dns.spoof.address (ip address) | set dns spoofing with IP Address |
| set dns.spoof.domains (domain) | set dns spoofing domain, ex. gmail.com,www.gmail.com,https://gmail.com |
| dns.spoof on | enable dns.spoof |

### PACK NAME

tools name :              Bettercap v2.32.0-1+b2 <br>
attack layer model (OSI): Layer 2 (ARP), Layer 3 (IP Address), Layer 1 (Wireless, or cabling)<br>
Description : <br>
Complete, modular, portable and easily extensible MITM framework <br>
 The Swiss Army knife for 802.11, BLE, IPv4 and IPv6 networks reconnaissance <br>
 and MITM attacks. <br>
 . <br>
 bettercap is a powerful, easily extensible and portable framework  written <br>
 in Go which aims to offer to security researchers, red teamers and reverse<br>
 engineers an easy to use, all-in-one solution with all the features they<br>
 might possibly need for performing reconnaissance and attacking WiFi<br>
 networks, Bluetooth Low Energy devices, wireless HID devices and Ethernet<br>
 networks.<br>
 .<br>
 Main Features:<br>
  * WiFi networks scanning, deauthentication attack, clientless PMKID
    association attack and automatic WPA/WPA2 client handshakes capture.<br>
  * Bluetooth Low Energy devices scanning, characteristics enumeration,
    reading and writing.<br>
  * 2.4Ghz wireless devices scanning and MouseJacking attacks with
    over-the-air HID frames injection (with DuckyScript support).<br>
  * Passive and active IP network hosts probing and recon.<br>
  * ARP, DNS, NDP and DHCPv6 spoofers for MITM attacks on IPv4 and IPv6
    based networks.<br>
  * Proxies at packet level, TCP level and HTTP/HTTPS application level
    fully scriptable with easy to implement javascript plugins.<br>
  * A powerful network sniffer for credentials harvesting which can also be
    used as a network protocol fuzzer.<br>
  * A very fast port scanner.<br>
  * A powerful REST API with support for asynchronous events notification
    on websocket to orchestrate your attacks easily.<br>
  * A very convenient web UI.<br>
  * More! (https://www.bettercap.org/modules/)<br>
 .<br>
 This package contains a Swiss Army knife for 802.11, BLE and Ethernet networks
 reconnaissance and attacks.<br>
<br>
<img src="https://user-images.githubusercontent.com/92193431/173983407-df81ef0a-a41a-46c2-abcb-97bb0db59875.jpeg" />
