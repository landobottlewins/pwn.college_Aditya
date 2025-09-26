
# Printing exported variables

## My solve
**Flag:** `pwn.college{o7xikqeAffUwuQLNSKLJ2l9XC2p.QX4UTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
HOSTNAME=variables~printing-exported-variables
PWD=/home/hacker
MANPATH=/run/dojo/share/man:
DOJO_AUTH_TOKEN=85b4ce77e18a33dced9ddebb1e7b5c25529e9cee8329bbd0fab8bf189e3ffc0f
HOME=/home/hacker
LANG=C.UTF-8
FLAG=pwn.college{o7xikqeAffUwuQLNSKLJ2l9XC2p.QX4UTN0wyM1gjNzEzW}
TERMINFO=/run/dojo/share/terminfo
TERM=xterm-256color
SHLVL=2
LC_CTYPE=C.UTF-8
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DEBIAN_FRONTEND=noninteractive
_=/run/dojo/bin/env
```

## Incorrect tangents I went on
None

## What I learned
using `env` to print every exported variable

## References 
None
