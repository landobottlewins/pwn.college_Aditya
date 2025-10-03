
# the SUID bit

## My solve
**Flag:** `pwn.college{wTjLD3v5INr7gj0mUPj-u81dTb1.QXwIDO0wyM1gjNzEzW}`

```bash
Connected!
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{YlpkQvGOm1CZ4QxQXoPWuFtfnE8.QXzEjN0wyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
giving root acess for a particular program using SUID bit with the command `chmod u+s`

## References 
None
