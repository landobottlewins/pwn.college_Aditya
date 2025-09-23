# Hidden files

## My solve
**Flag:** `pwn.college{0zzGZWcjpp-cmBUjlo_ju29bJid.QXwUDO0wyM1gjNzEzW}`

```bash
Connected!
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.           .flag-3339211545672  challenge  home   lib64   mnt  proc  sbin  tmp
..          bin                  dev        lib    libx32  nix  root  srv   usr
.dockerenv  boot                 etc        lib32  media   opt  run   sys   var
hacker@commands~hidden-files:/$ cat .flag-3339211545672
pwn.college{0zzGZWcjpp-cmBUjlo_ju29bJid.QXwUDO0wyM1gjNzEzW}
```

## Incorrect tangents I went on
didn't `cd \` instead directly typed `ls -a`

## What I learned
`ls` doesnt list all files by default (such as hidden files).
We can use  `ls -a` to show all files.

## References 
None
