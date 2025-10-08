# Reading shell scripts 

## My solve
**Flag:** `pwn.college{oSDNaiI0bMDv9dYVCyCRCJ7r6ey.0lMwgDOxwyM1gjNzEzW}`

```bash
Connected!
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ /challenge/run
hack the PLANET
CORRECT! Your flag:
pwn.college{oSDNaiI0bMDv9dYVCyCRCJ7r6ey.0lMwgDOxwyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
reading a shell script using `cat`

## References 
None
