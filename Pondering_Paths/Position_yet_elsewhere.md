# Position yet elsewhere

## My solve
**Flag:** `pwn.college{Iif_8sJbYA3Lh2hAgaIMcTCxxBo.QX4QTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /proc/131 directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /proc/131
hacker@paths~position-yet-elsewhere:/proc/131$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Iif_8sJbYA3Lh2hAgaIMcTCxxBo.QX4QTN0wyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
Can change working directory of a process using `cd` command

## References 
None
