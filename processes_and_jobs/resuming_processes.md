# resuming processes

## My solve
**Flag:** `pwn.college{g0IGFLxTZqWQORQhqjEVa9deFTc.QX2QDO0wyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with 
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg /challenge/run
/challenge/run
I'm back! Here's your flag:
pwn.college{g0IGFLxTZqWQORQhqjEVa9deFTc.QX2QDO0wyM1gjNzEzW}
Don't forget to press Enter to quit me!

Goodbye!

```

## Incorrect tangents I went on
none

## What I learned
resuming a suspended program using `fg`

## References 
None
