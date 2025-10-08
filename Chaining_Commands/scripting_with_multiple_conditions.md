# Scripting with multiple conditions 

## My solve
**Flag:** `pwn.college{MFgIvZU9vIRToLZXV5LyUMNQjkP.0FOzMDOxwyM1gjNzEzW}`

```bash
Connected!
hacker@chaining~scripting-with-multiple-conditions:~$ nano solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{MFgIvZU9vIRToLZXV5LyUMNQjkP.0FOzMDOxwyM1gjNzEzW}
```
in the solve.sh file
```
if [ "$1" == "hack" ]
then
        echo "the planet"
elif [ "$1" == "pwn" ]
then
        echo "college"
elif [ "$1" == "learn" ]
then
        echo "linux"
else
        echo "unknown"
fi
```


## Incorrect tangents I went on
none

## What I learned
scripting multiple conditions using elif and its syntax

## References 
None
