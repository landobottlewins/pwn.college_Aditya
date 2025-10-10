# Adding Commands

## My solve
**Flag:** `pwn.college{UPnG-nm5EaU6zD0kIURhjSsNXhd.QX2cjM1wyM1gjNzEzW}`

```bash
Connected!
hacker@path~adding-commands:~$ nano win
hacker@path~adding-commands:~$ chmod +x win
hacker@path~adding-commands:~$ PATH=. /challenge/run
Invoking 'win'....
pwn.college{UPnG-nm5EaU6zD0kIURhjSsNXhd.QX2cjM1wyM1gjNzEzW}
```
in the win bash script
```bash
#!/bin/sh
/bin/cat /flag
```

## Incorrect tangents I went on
None

## What I learned
adding new commands using the PATH

## References 
Since `win` won't be able to find `cat` if I change the `PATH`, I asked chatgpt how to set PATH for only one command and reset for the next. 
Hence I used `PATH=. /challenge/run`
