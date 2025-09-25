# Redirecting input

## My solve
**Flag:** `pwn.college{8fdoaTiv557Fx_h9wTuthK0tYpN.QXwcTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{8fdoaTiv557Fx_h9wTuthK0tYpN.QXwcTN0wyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
redirecting output using `>` and input using `<`

## References 
None
