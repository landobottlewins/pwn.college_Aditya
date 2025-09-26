# named pipes

## My solve
**Flag:** `pwn.college{I07-RCWB2gDdOEjpbpG3Zc9FopQ.0FOxEzNxwyM1gjNzEzW}`

```bash
Connected!
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
```

other terminal 
```bash
aditya@Dell-Inspiron:~$ ssh -i key hacker@dojo.pwn.college
Connected!
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here is your flag:
pwn.college{UCMuGDykp_jxFKeB_rP-5zihixy.01MzMDOxwyM1gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@piping~named-pipes:~$ touch /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
WARNING: /tmp/flag_fifo is not a FIFO! Use mkfifo to make it!
The stdout of /challenge/run does not seem to point to a FIFO!
```

## What I learned
create and use FIFOs (named pipes) with the `mkfifo` command.

## References 
None
