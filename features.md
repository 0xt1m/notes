# Features
### Upgrade reverse-shell
```
python -c 'import pty; pty.spawn("/bin/bash")'
# Ctrl+Z
stty raw -echo && fg
reset
xterm
```
### Nmap
`-min-rate=10000` to speed up `nmap` scan.


### spawn a reverse-shell
```
/bin/bash -p
```