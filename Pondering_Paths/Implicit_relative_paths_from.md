# Implicit relative paths, from /

## My solve
**Flag:** `pwn.college{wnZ24IoGcgMoESMIw3fgoTXuezn.QX5QTN0wyM1gjNzEzW}`

```bash
Connected!
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{wnZ24IoGcgMoESMIw3fgoTXuezn.QX5QTN0wyM1gjNzEzW}
```

## Incorrect tangents I went on
tried `/challenge/run` after executing `cd /`
which gave the hint to what I was supposed to do
```bash
hacker@paths~implicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
```

## What I learned
relative paths and how to work with them

## References 
None
