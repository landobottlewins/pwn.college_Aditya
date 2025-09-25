# Redirecting more output

## My solve
**Flag:** `pwn.college{g7txUCBBAVSyJqBYMTucdp09GsD.QX1YTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{g7txUCBBAVSyJqBYMTucdp09GsD.QX1YTN0wyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
we can redirect the output of any command to a file using `>`

## References 
None
