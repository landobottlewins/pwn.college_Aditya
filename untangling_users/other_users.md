# Other users with su

## My solve
**Flag:** `pwn.college{AXxBy-Ha-SDCfyF7eFiJqevRYxC.QX2UDN1wyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@users~other-users-with-su:~$ su zardus
Password: 
zardus@users~other-users-with-su:/home/hacker$ cat /flag
cat: /flag: Permission denied
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{AXxBy-Ha-SDCfyF7eFiJqevRYxC.QX2UDN1wyM1gjNzEzW}

```

## Incorrect tangents I went on
none

## What I learned
switching to another user using `su`

## References 
None
