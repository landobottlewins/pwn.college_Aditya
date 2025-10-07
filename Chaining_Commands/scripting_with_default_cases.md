# scripting with default cases 

## my solve
**Flag:** `pwn.college{ADWInyDN5uEaEbylkNp55VNLV0n.01NzMDOxwyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@chaining~scripting-with-default-cases:~$ nano solve.sh
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{ADWInyDN5uEaEbylkNp55VNLV0n.01NzMDOxwyM1gjNzEzW}


```

in the solve.sh file
```                                    
#!/bin/bash
if [ "$1" == "pwn" ]
then
    echo "college"
else
    echo "nope"
fi
```

## Incorrect tangents I went on
None

## What I learned
scripting for if else in bash script and its syntax


## References 
None
