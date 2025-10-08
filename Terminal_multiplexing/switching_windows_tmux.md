
# Switching windows (tmux)

## My solve
**Flag:** `pwn.college{I-PnvTHufeyHjfNzGX_Dv4Lu51A.0FM5IDOxwyM1gjNzEzW}`

```bash
Connected!
hacker@terminal-multiplexing~switching-windows-tmux:~$ tmux ls
challenge_session: 2 windows (created Wed Oct  8 07:39:35 2025)
hacker@terminal-multiplexing~switching-windows-tmux:~$ tmux a
[detached (from session challenge_session)]
```

```bash
 cat <<MSG
Welcome to the tmux window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-B 0 to switch to window 0!
MSG
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Welcome to the tmux window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-B 0 to switch to window 0!
> MSG
Welcome to the tmux window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-B 0 to switch to window 0!
```

```bash
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{I-PnvTHufeyHjfNzGX_Dv4Lu51A.0FM5IDOxwyM1gjNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{I-PnvTHufeyHjfNzGX_Dv4Lu51A.0FM5IDOxwyM1gjNzEzW}
hacker@terminal-multiplexing~switching-windows-tmux:~$
```

## Incorrect tangents I went on
None

## What I learned
switching through windows in tmux

## References 
None
