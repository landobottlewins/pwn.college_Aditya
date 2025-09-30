# Catting absolute paths

## My solve
**Flag:** `pwn.college{4cFNyovljJm6AVNPxDb6nVGQBwp.QX5YDO1wyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
148
hacker@processes~process-exit-codes:~$ /challenge/submit-code 148
CORRECT! Here is your flag:
pwn.college{4cFNyovljJm6AVNPxDb6nVGQBwp.QX5YDO1wyM1gjNzEzW}

```

## Incorrect tangents I went on
none

## What I learned
reading exit code using `$?`

## References 
None
