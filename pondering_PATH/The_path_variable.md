# The path variable

## My solve
**Flag:** `pwn.college{UyydJ6pC1CpTtgKXaCzW7kUD4vV.QX2cDM1wyM1gjNzEzW}`

```bash
Connected!
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{UyydJ6pC1CpTtgKXaCzW7kUD4vV.QX2cDM1wyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
- PATH stores a bunch of directory paths in which the shell will search for programs corresponding to commands
- Without a PATH, bash cannot find the ls command.

## References 
None
