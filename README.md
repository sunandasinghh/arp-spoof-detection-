# arp-spoof-detection-using-wirehark
a simple demonstration of a local arp-spoofing attack , using a virtual kali machine.
## objectives
  stimulate and record arp spoofing behaviour using wireshark to understand:
    -arp request and reply machines 
    -how spoofed arp replies posion to victims ARP ache
    -how to detect such apps with packet inspection

##lab setup
  - **Host OS**: Windows 11
  - **VM Software**: Oracle VirtualBox
  - **Guest VM**: Kali Linux 2024.4
  - **Networking Mode**: NAT (shared local network)
  - **Tool Used**: `arpspoof` from the `dsniff` package
  - **Packet Capture Tool**: Wireshark

1. Kali (attacker): Run Wireshark on `eth0`
2. Identify target and gateway IPs (`ip a`, `ip r`, `ip neigh`)
3. Launch ARP spoof:
   ```bash
   arpspoof -i eth0 -t 192.168.0.105 192.168.0.
    
  
