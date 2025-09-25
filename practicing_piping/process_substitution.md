
# Redirecting input

## My solve
**Flag:** `pwn.college{czMCHSYJv7mUQG7dkVODXQ5uxIT.0lNwMDOxwyM1gjNzEzW}`

```bash
Connected!
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
51a52
> pwn.college{czMCHSYJv7mUQG7dkVODXQ5uxIT.0lNwMDOxwyM1gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
Process substitution using `<(...)` command. Basically treating a commmand as a file.

## References 
None
