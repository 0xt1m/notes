# BlueTeaming

## Centos
Install `pstree`
```
sudo yum install psmisc
```

### Useful commands:
**To see active shells.**
```
who
```

**To see process tree**
```
pstree -p
```

**To see all the processes**
```
ps aux
```

**To see info about specific process**
```
ps aux | grep "<PID>"
```

**To kill process**
```
kill <pid> # gracefully
kill -9 <pid> # forcefully
```
