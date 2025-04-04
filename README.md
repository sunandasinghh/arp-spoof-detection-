# arp-spoof-detection-using-wirehark
a simple detection of arp spoofing on local network and how to detect it using wireshark.
ENVIRONMENT USED AS FOLLOWS:
  -Kali linux (Virtual Machine)
  -Another device in the same LAN
  -Wireshark
TARGET IPS:
  - Router: `192.168.1.1`
  - Victim device: `192.168.1.3` (host machine or VM)

`bash
 Terminal 1: Pretend to be router to victim
sudo arpspoof -i eth0 -t 192.168.1.3 192.168.1.1
  
