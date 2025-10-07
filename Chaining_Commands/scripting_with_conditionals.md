# scripting with conditionals

## my solve
**Flag:** `pwn.college{cizQ6HWd-Py43mlKFVZe-cs4XPc.0lNzMDOxwyM1gjNzEzW}`

```bash
Connected!
hacker@chaining~scripting-with-conditionals:~$ nano solve.sh
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{cizQ6HWd-Py43mlKFVZe-cs4XPc.0lNzMDOxwyM1gjNzEzW}

```
in solve.sh file
```
  GNU nano 8.4                                       solve.sh                                                 
#!/bin/bash
if [ "$1" == "pwn" ]
then
    echo "college"
fi
```

## Incorrect tangents I went on
None

## What I learned
using `if` in bash script and its syntax

## References 
None
