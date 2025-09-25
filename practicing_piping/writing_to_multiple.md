
# Writing to multiple programs

## My solve
**Flag:** `pwn.college{AtNw_lWxu4DTISzKe_8j2DEYquN.QXwgDN1wyM1gjNzEzW}`

```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
16865211432679923727
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{AtNw_lWxu4DTISzKe_8j2DEYquN.QXwgDN1wyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
using the `tee` command to view data flowing through a pipe

## References 
None
