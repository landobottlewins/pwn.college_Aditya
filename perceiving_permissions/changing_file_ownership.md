# Catting absolute paths

## My solve
**Flag:** `pwn.college{4VV1-kYAbjVt4MuZO50uSkcdMlt.QXxEjN0wyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{4VV1-kYAbjVt4MuZO50uSkcdMlt.QXxEjN0wyM1gjNzEzW}

```

## Incorrect tangents I went on
none

## What I learned
-using `ls -l` to see owner of a file
-changing owner of a file using `chown`

## References 
None
