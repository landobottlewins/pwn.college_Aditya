
# Duplicating piped data with tee

## My solve
**Flag:** `pwn.college{8fdoaTiv557Fx_h9wTuthK0tYpN.QXwcTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee a | /challenge/college
Processing...
WARNING: you are overwriting file a with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat a
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "4QhSjUdi"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret 4QhSjUdi | tee a | /challenge/college
Processing...
WARNING: you are overwriting file a with tee's output...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{4QhSjUdi5AhelGhRp_P_4WlQQ3D.QXxITO0wyM1gjNzEzW}
```

## Incorrect tangents I went on
```Bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret 4QhSjUdi | tee /challenge/college
Processing...
You are trying to use 'tee' *instead* of /challenge/college. Use it *between*
/challenge/pwn and /challenge/college!
You must pipe the output of /challenge/pwn into /challenge/college (or 'tee'
for debugging).
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret 4QhSjUdi
Processing...
You must pipe the output of /challenge/pwn into /challenge/college (or 'tee'
for debugging).
```

## What I learned
using the `tee` command to view data flowing through a pipe

## References 
None
