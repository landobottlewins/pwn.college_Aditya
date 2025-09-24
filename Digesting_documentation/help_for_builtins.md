# Help for builtins

## My solve
**Flag:** `pwn.college{cszKczR1Kib4zVwOadQsbq3YoQh.QX0ETO0wyM1gjNzEzW}`

```bash
Connected!
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "cszKczR1".
hacker@man~help-for-builtins:~$ challenge --secret cszKczR1
Correct! Here is your flag!
pwn.college{cszKczR1Kib4zVwOadQsbq3YoQh.QX0ETO0wyM1gjNzEzW}

```

## Incorrect tangents I went on
none

## What I learned
For some commands help options, are built into the shell itself known as builtins

## References 
None
