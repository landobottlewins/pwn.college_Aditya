# Catting absolute paths

## My solve
**Flag:** `pwn.college{kNMbNYqPNSJ7bnH9rdRdaepO3XF.QXyQDO0wyM1gjNzEzW}`

```bash
connected!                                                                        
hacker@processes~killing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   20:21   0:00 /sbin/docker-init -- /nix/var/nix/profiles/
root           7  0.0  0.0 231708  2560 ?        S    20:21   0:00 /run/dojo/bin/sleep 6h
root         136  0.0  0.0   5204  3520 ?        S    20:21   0:00 su -c /challenge/.launcher hacker
hacker       137  0.0  0.0 231576  3520 ?        Ss   20:21   0:00 /challenge/dont_run
hacker       138  0.0  0.0 231708  2560 ?        S    20:21   0:00 sleep 6h
hacker       140  0.0  0.0 231576  3520 pts/0    Ss   20:21   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1
hacker       146  0.0  0.0 231940  4160 pts/0    S    20:21   0:00 /run/dojo/bin/bash --login
hacker       157  0.0  0.0 233600  3840 pts/0    R+   20:27   0:00 ps aux
hacker@processes~killing-processes:~$ kill 137
hacker@processes~killing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   20:21   0:00 /sbin/docker-init -- /nix/var/nix/profiles/
root           7  0.0  0.0 231708  2560 ?        S    20:21   0:00 /run/dojo/bin/sleep 6h
hacker       138  0.0  0.0 231708  2560 ?        S    20:21   0:00 sleep 6h
hacker       140  0.0  0.0 231576  3520 pts/0    Ss   20:21   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1
hacker       146  0.0  0.0 231940  4160 pts/0    S    20:21   0:00 /run/dojo/bin/bash --login
hacker       162  0.0  0.0 233600  3840 pts/0    R+   20:28   0:00 ps aux
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{kNMbNYqPNSJ7bnH9rdRdaepO3XF.QXyQDO0wyM1gjNzEzW}

```

## Incorrect tangents I went on
none

## What I learned
killing processes using the kill command

## References 
None
