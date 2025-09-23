# Implicit relative path

## My solve
**Flag:** `pwn.college{A47pYY0EULwYAmRCNo0_bSq1CmU.QXxUTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{A47pYY0EULwYAmRCNo0_bSq1CmU.QXxUTN0wyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path.
Had I run the command `run` instead of `./run` here, linux would not have invoked the `/challenge/run`. 
This is a safety measure.

## References 
None
