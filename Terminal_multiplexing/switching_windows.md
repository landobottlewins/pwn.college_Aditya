
# switching windows

## My solve
**Flag:** `pwn.college{E-psSWOg08GUfK86Y3rZlPrN3KA.0FO4IDOxwyM1gjNzEzW}`

```bash
hacker@terminal-multiplexing~switching-windows:~$ screen -ls
There are screens on:
        150.pts-0.terminal-multiplexing~launching-screen        (Remote or dead)
        144.session_c82ca891b6e25d32    (Remote or dead)
        147.session_a5c6eb2def9e8d25    (Remote or dead)
        150.session_b4b5b3aed0fbcb22    (Remote or dead)
        135.challenge_session   (Detached)
        174.pts-2.terminal-multiplexing~switching-windows       (Detached)
6 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~switching-windows:~$ screen -r 135.challenge_session
[detached from 135.challenge_session]
```

```bash
 cat <<MSG
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!
MSG
hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Welcome to the window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-A 0 to switch to window 0!
> MSG
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!
```

```bash
hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{E-psSWOg08GUfK86Y3rZlPrN3KA.0FO4IDOxwyM1gjNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{E-psSWOg08GUfK86Y3rZlPrN3KA.0FO4IDOxwyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
switching through the multiple windows in terminal using keyboard shortcuts

## References 
None
