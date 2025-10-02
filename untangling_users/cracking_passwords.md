# Cracking passwords

## My solve
**Flag:** `pwn.college{MOut6raFuHuctvj0GhIrRMGAe_S.QX3UDN1wyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04835g/s 281.5p/s 281.5c/s 281.5C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password: 
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{MOut6raFuHuctvj0GhIrRMGAe_S.QX3UDN1wyM1gjNzEzW}

```

## Incorrect tangents I went on
none

## What I learned
cracking i.e. unencrypting stored passwords using "John the Ripper" `john`

## References 
None
