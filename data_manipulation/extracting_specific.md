# Extracting specific sections of text

## My solve
**Flag:** `pwn.college{s5LEsGQ_piwDhk6qlD_TIGt8BpQ.01NxEzNxwyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d ' ' -f 2 | tr -d '\n'
pwn.college{s5LEsGQ_piwDhk6qlD_TIGt8BpQ.01NxEzNxwyM1gjNzEzW}
```

## Incorrect tangents I went on
none

## What I learned
using `-cut` to extract columns

## References 
None
