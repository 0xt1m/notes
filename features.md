# Features
### Upgrade reverse-shell
```
python -c 'import pty; pty.spawn("/bin/bash")'
# Ctrl+Z
stty raw -echo && fg
reset
xterm
```

### spawn a reverse-shell
```
/bin/bash -p
```