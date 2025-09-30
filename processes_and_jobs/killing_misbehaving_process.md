# killing misbehaving process

## My solve
**Flag:** `pwn.college{URs2SY-BBsCktqtVmVYHKw3jceH.0FNzMDOxwyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@processes~killing-misbehaving-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.6  0.0   1056   640 ?        Ss   22:44   0:00 /sbin/docker-init -- /nix/var/nix/profiles/
root           7  0.3  0.0 231708  2560 ?        S    22:44   0:00 /run/dojo/bin/sleep 6h
root         137  0.0  0.0   4132  1280 ?        S    22:44   0:00 /bin/bash /challenge/.init
root         138  0.0  0.0   4132  1280 ?        S    22:44   0:00 /bin/bash /challenge/.init
root         139  0.0  0.0   5204  3520 ?        S    22:44   0:00 su -c exec /challenge/decoy > /tmp/flag_fif
root         140  0.0  0.0   2744  1600 ?        S    22:44   0:00 sleep 6h
root         141  0.0  0.0   2744  1280 ?        S    22:44   0:00 sleep 6h
hacker       142  0.7  0.0  13516  9600 ?        Ss   22:44   0:00 /usr/bin/python /challenge/decoy
hacker       144  0.9  0.0 231576  3520 pts/0    Ss   22:44   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1
hacker       150  0.0  0.0 231972  4160 pts/0    S    22:44   0:00 /run/dojo/bin/bash --login
hacker       159  0.0  0.0 233600  3840 pts/0    R+   22:44   0:00 ps aux
hacker@processes~killing-misbehaving-processes:~$ kill 142
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
```
in another terminal 
```bash
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
```
```
pwn.college{URs2SY-BBsCktqtVmVYHKw3jceH.0FNzMDOxwyM1gjNzEzW}
```



## Incorrect tangents I went on
none

## What I learned
finding misbehaving program

## References 
None
