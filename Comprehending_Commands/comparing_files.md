# Comparing files

## My solve
**Flag:** `pwn.college{QHKMM10UYruMxUGN-rJU8L0R9vc.01MwMDOxwyM1gjNzEzW}`

```bash
Connected!
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
79a80
> pwn.college{QHKMM10UYruMxUGN-rJU8L0R9vc.01MwMDOxwyM1gjNzEzW}
```

## Incorrect tangents I went on
none

## What I learned
Comparing files using the diff command. To find the uncommon elements between two files we can run command `diff file1 file2` and find the elements.

## References 
None
