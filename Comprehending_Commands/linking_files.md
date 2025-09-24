# LInking files

## My solve
**Flag:** `pwn.college{gKgFEBoI-dxBhh0o4iVRcKOhECV.QX5ETN1wyM1gjNzEzW}`

```bash
Connected!
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{gKgFEBoI-dxBhh0o4iVRcKOhECV.QX5ETN1wyM1gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@commands~linking-files:~$ ln -s /challenge/catflag /home/hacker/new
hacker@commands~linking-files:~$ cat new
#!/opt/pwn.college/bash

fold -s <<< "About to read out the /home/hacker/not-the-flag file!"
cat /home/hacker/not-the-flag
```

## What I learned
linking files using `ln`. Using the `ln -s` command creates a symlink.

## References 
None
