# listing processes

## My solve
**Flag:** `pwn.college{UG1RrGztUVLm0imsf_pXYv302zr.QX4MDO0wyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   20:09   0:00 /sbin/docker-init -- /nix/var/nix/profiles/
root           7  0.0  0.0 231708  2560 ?        S    20:09   0:00 /run/dojo/bin/sleep 6h
root         132  0.0  0.0   4132  2560 ?        S    20:09   0:00 /challenge/31483-run-8998
root         135  0.0  0.0   2744  1600 ?        S    20:09   0:00 sleep 6h
hacker       137  0.0  0.0 231576  3520 pts/0    Ss   20:10   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1
hacker       143  0.0  0.0 231940  4160 pts/0    S    20:10   0:00 /run/dojo/bin/bash --login
hacker       152  0.0  0.0 233600  3840 pts/0    R+   20:14   0:00 ps aux
hacker@processes~listing-processes:~$ /challenge/31483-run-8998
Yahaha, you found me! Here is your flag:
pwn.college{UG1RrGztUVLm0imsf_pXYv302zr.QX4MDO0wyM1gjNzEzW}
Now I will sleep for a while (so that you could find me with 'ps').

```

## Incorrect tangents I went on
none

## What I learned
list the processes running using `ps` and '-ef` or `aux` to list all of them 

## References 
None
