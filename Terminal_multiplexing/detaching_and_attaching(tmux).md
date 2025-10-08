# detaching and attaching (tmux)

## My solve
**Flag:** `pwn.college{QvgguuUH5q5nFqPk3iJSA3FpL7p.0VO4IDOxwyM1gjNzEzW}`

```bash
Connected!
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux
[detached (from session 0)]
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ /challenge/run
Found detached tmux session: 0
Sending flag to your tmux session...

Flag sent! Now reattach to your tmux session with:
  tmux attach

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux a
[exited]
```

```bash
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$  echo Congratulations, here is your flag: pwn.college{QvgguuUH5q5nFqPk3iJSA3FpL7p.0VO4IDOxwyM1gjNzEzW}
Congratulations, here is your flag: pwn.college{QvgguuUH5q5nFqPk3iJSA3FpL7p.0VO4IDOxwyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
- tmux is similar to to screen
- use ctrl b instead of a for activation key
- tmux ls - List sessions
- tmux attach or tmux a - Reattach to session


## References 
None
