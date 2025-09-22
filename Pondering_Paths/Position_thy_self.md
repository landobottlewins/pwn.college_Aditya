# Position thy self 

## My solve
**Flag:** `pwn.college{8dfLqetxj1rj1ZVNC_b4GlNWp7e.QX2QTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/aarch64-linux-gnu/include/gnu directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd  /usr/aarch64-linux-gnu/include/gnu
hacker@paths~position-thy-self:/usr/aarch64-linux-gnu/include/gnu$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{8dfLqetxj1rj1ZVNC_b4GlNWp7e.QX2QTN0wyM1gjNzEzW}
```

## Incorrect tangents I went on
tried `cd /challenge/run` but realised that I needed to find specific path (according to the challenge statement)

## What I learned
Can change working directory of a process using `cd` command

## References 
None

