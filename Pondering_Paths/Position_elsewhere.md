# Position elsewhere

## My solve
**Flag:** `pwn.college{cLIkTwkcpYiX0LKlUCOb0NnJkzx.QX3QTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /sys/kernel directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /sys/kernel
hacker@paths~position-elsewhere:/sys/kernel$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{cLIkTwkcpYiX0LKlUCOb0NnJkzx.QX3QTN0wyM1gjNzEzW}
```

## Incorrect tangents I went on
None, since I realised it is similar to the previous challenge.

## What I learned
Can change working directory of a process using `cd` command

## References 
Previous problem "position thy self"
