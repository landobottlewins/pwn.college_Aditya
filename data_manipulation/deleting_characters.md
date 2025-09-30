# deleting characters

## My solve
**Flag:** `pwn.college{kycTVm_50yQs7KaEsCsLnAssAJU.0FNxEzNxwyM1gjNzEzW}`

```bash
Connected!                                                                        
hacker@data~deleting-characters:~$ /challenge/run | tr -d ^%
Your character-stuffed flag:
pwn.college{kycTVm_50yQs7KaEsCsLnAssAJU.0FNxEzNxwyM1gjNzEzW}

```

## Incorrect tangents I went on
put a space between `^` and `%`
```bash
Connected!                                                                        
hacker@data~deleting-characters:~$ /challenge/run | tr -d ^ %
tr: extra operand ‘%’
Only one string may be given when deleting without squeezing repeats.
Try 'tr --help' for more information.
```

## What I learned
deleting characters using `tr -d`

## References 
None
