# Grepping stored results

## My solve
**Flag:** `pwn.college{8-DY4UxNRGJFf7YbAODeP6-mudw.QX4EDO0wyM1gjNzEzW}`

```bash
Connected!
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep pwn.college /tmp/data.txt
pwn.college{8-DY4UxNRGJFf7YbAODeP6-mudw.QX4EDO0wyM1gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@piping~grepping-stored-results:~$ grep "flag" /tmp/data.txt
[FLAG] Here is your flag:
flagellate
flagged
flagrant
flagstaff's
unflagging
conflagration
flagellating
flagons
flagellated
conflagration's
flagrantly
flagellation's
flagpoles
flagstaff
camouflaging
flagstone's
camouflage's
flagellums
flagpole's
flagship's
flagon
flagging
flags
flagellation
persiflage
flagships
flagella
camouflaged
persiflage's
camouflage
flag
flagstaffs
camouflages
flagellum
flagship
flagstone
flagon's
flagstones
flagellum's
flag's
conflagrations
flagpole
flagellates
```
## What I learned
redirecting output using `>` and file searching using `grep`

## References 
None
