
# Exporting variables

## My solve
**Flag:** `pwn.college{k00icwQ259e4sPfhBa0LJL_iwHa.QXyYTN0wyM1gjNzEzW}`

```bash
Connected!
EXhacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{k00icwQ259e4sPfhBa0LJL_iwHa.QXyYTN0wyM1gjNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```

## Incorrect tangents I went on
None

## What I learned
using `export` to make variable visible to other program

## References 
None
