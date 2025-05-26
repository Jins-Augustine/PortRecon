# PortRecon

---

## Objective  
Scan local subnet (192.168.88.0/24) to find devices & open ports.

## Tools  
- Nmap (TCP SYN scan)  
- Kali Linux terminal

## Command  
```bash
nmap -sS 192.168.88.0/24 -oN nmap_scan.txt
```


| IP             | Open Ports          | Service | Notes           |
| -------------- | ------------------- | ------- | --------------- |
| 192.168.88.2   | 53/tcp              | DNS     | Domain service  |
| 192.168.88.128 | 22/tcp              | SSH     | Kali Linux VM   |
|                | 443/tcp (filtered)  | HTTPS   | Port filtered   |
|                | 9200/tcp (filtered) | wap-wsp | Port filtered   |
| 192.168.88.254 | All ports filtered  | N/A     | Router/Firewall |


