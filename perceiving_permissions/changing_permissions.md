# Changing permissions

## My solve
**Flag:** `pwn.college{4QCPPl-90F3x7biWdkaVPSfDleY.QXzcjM1wyM1gjNzEzW}`

```bash
Connected!
hacker@permissions~changing-permissions:~$ chmod o+wrx /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{4QCPPl-90F3x7biWdkaVPSfDleY.QXzcjM1wyM1gjNzEzW}

```
chmod `o+r` would also do the same

## Incorrect tangents I went on
`chmod u+wrx /flag`
the owner is root not hacker

## What I learned
changing permissions of a file using `chmod` 

## References 
None
