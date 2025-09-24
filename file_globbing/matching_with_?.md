# Matching with ? 

## My solve
**Flag:** `pwn.college{06wj5LblWEGCSNyTV1MvFbYw0zC.QXyIDO0wyM1gjNzEzW}`

```bash
Connected!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /?????????
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{06wj5LblWEGCSNyTV1MvFbYw0zC.QXyIDO0wyM1gjNzEzW}

```

## Incorrect tangents I went on
none

## What I learned
globbing with `?`
When the shell encounters a `?` character in any argument, the shell will treat it as a single-character wildcard. This works like `*`, but only matches one character.

## References 
None
