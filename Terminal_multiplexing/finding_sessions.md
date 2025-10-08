
# finding sessions

## My solve
**Flag:** `pwn.college{AzBKj9wKwOCamVgESaPRgt6Cymd.01N4IDOxwyM1gjNzEzW}`

```bash
Connected!
hacker@terminal-multiplexing~finding-sessions:~$ screen -ls
There are screens on:
        150.pts-0.terminal-multiplexing~launching-screen        (Remote or dead)
        144.session_c82ca891b6e25d32    (Detached)
        147.session_a5c6eb2def9e8d25    (Detached)
        150.session_b4b5b3aed0fbcb22    (Detached)
4 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r  150.pts-0.terminal-multiplexing~launching-screen
There is a screen on:
        150.pts-0.terminal-multiplexing~launching-screen        (Dead ???)
Remove dead screens with 'screen -wipe'.
There is no screen to be resumed matching 150.pts-0.terminal-multiplexing~launching-screen.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r 144.session_c82ca891b6e25d32
[detached from 144.session_c82ca891b6e25d32]
```

```bash
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Congratulations! You found the right session!'
Congratulations! You found the right session!
hacker@terminal-multiplexing~finding-sessions:~$  echo pwn.college{AzBKj9wKwOCamVgESaPRgt6Cymd.01N4IDOxwyM1gjNzEzW}
pwn.college{AzBKj9wKwOCamVgESaPRgt6Cymd.01N4IDOxwyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
- listing active terminals
- connecting to specific terminal

## References 
None
