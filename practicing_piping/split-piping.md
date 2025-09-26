
# Split-piping stderr and stdout

## My solve
**Flag:** `pwn.college{w80s67ILfvfHXwFyi66EynItYW3.QXxQDM2wyM1gjNzEzW}`

```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >(/challenge/the) | /challenge/planet
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{w80s67ILfvfHXwFyi66EynItYW3.QXxQDM2wyM1gjNzEzW}
```

## Incorrect tangents I went on
```bash
Connected!
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> /challenge/the | /challenge/planet
bash: /challenge/the: Permission denied
Are you sure you're properly redirecting /challenge/hack's standard output into
'/challenge/planet'?
```

```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >(/challenge/the) | >(/challenge/planet)
bash: /dev/fd/63: Permission denied
Are you sure you're properly redirecting /challenge/hack's standard output into
'/challenge/planet'?
```


## What I learned
revision of previous challenges

## References 
None
