# Nmap

- **Gives services and their versions**
```
nmap -sC -sV <ip>
```

- **Scan all the ports**
```
nmap -p- <ip>
```

- **Speed up nmap scan**
```
nmap -min-rate=10000 -p- <ip>
```