# Redirecting script output

## my solve
**Flag:** `pwn.college{4fKbSWuyCw6bteClW-gsumz3RfF.QX4ETO0wyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@chaining~redirecting-script-output:~$ touch x.sh
hacker@chaining~redirecting-script-output:~$ nano x.sh
hacker@chaining~redirecting-script-output:~$ nano x.sh
hacker@chaining~redirecting-script-output:~$ bash x.sh | > /challenge/solve
bash: /challenge/solve: Permission denied
It looks like you are not piping this script out to /challenge/solve! Remember 
to pipe the output of your script into /challenge/solve using '|'.
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{4fKbSWuyCw6bteClW-gsumz3RfF.QX4ETO0wyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
redirecting output of a bash script with piping `|`

## References 
None
