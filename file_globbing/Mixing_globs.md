# Mixing globs

## My solve
**Flag:** `pwn.college{QuvjU96TuNdXt77Q49XIrBzjHHI.QX1IDO0wyM1gjNzEzW}`

```bash
Connected!
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *i*n*
Error: you did not use a square bracket glob...
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{QuvjU96TuNdXt77Q49XIrBzjHHI.QX1IDO0wyM1gjNzEzW}

```

## Incorrect tangents I went on
challenging, educational, pwning have "i" "n" in common
```bash
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *i*n*
Error: you did not use a square bracket glob...
```

## What I learned
mixing globing using `[]` and `*`

## References 
None
