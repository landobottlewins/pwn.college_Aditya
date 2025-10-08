
# detaching and attaching

## My solve
**Flag:** `pwn.college{wTjLD3v5INr7gj0mUPj-u81dTb1.QXwIDO0wyM1gjNzEzW}`

```bash
Connected!
hacker@terminal-multiplexing~detaching-and-attaching:~$
Connected!
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen
[detached from 139.pts-0.terminal-multiplexing~detaching-and-attaching]
hacker@terminal-multiplexing~detaching-and-attaching:~$
hacker@terminal-multiplexing~detaching-and-attaching:~$ /challenge/run
Found detached screen session: 139.pts-0.terminal-multiplexing~detaching-and-attaching
Sending flag to your screen session...

Flag sent! Now reattach to your screen session with:

  screen -r

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen -r
[screen is terminating]
```
```bash
hacker@terminal-multiplexing~detaching-and-attaching:~$ echo Yes! Flag is: pwn.college{sZmQH1Qtowa5VpoM56xDIGfQsIo.0lN4IDOxwyM1gjNzEzW}
Yes! Flag is: pwn.college{sZmQH1Qtowa5VpoM56xDIGfQsIo.0lN4IDOxwyM1gjNzEzW}
```


## Incorrect tangents I went on
none

## What I learned
-detaching a terminal using `ctrl`+`a` and `d`
-reattaching using `screen -r`

## References 
None
