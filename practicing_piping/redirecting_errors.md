# Redirecting errors

## My solve
**Flag:** `pwn.college{k79jqvhbVMkqfBqDq_EhxKxXY2_.QX3YTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat instructions
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will check that error output is redirected to a specific file path : instructions
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!

[TEST] You should have redirected my stderr to instructions. Checking...

[PASS] The file at the other end of my stderr looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{k79jqvhbVMkqfBqDq_EhxKxXY2_.QX3YTN0wyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
redirecting output using `>` and errors using `2>`, here 1 and 2 stand as follows:
FD 1: Standard Output
FD 2: Standard Error

## References 
None
