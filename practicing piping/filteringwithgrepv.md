# Filtering with grep -v

**Flag:** pwn.college{4vY-KcK4kCIzuvzJ_jolwGUT4vJ.0FOxEzNxwyM1AzNzEzW}

**What I learnt:**  grep -v shows lines that do NOT match a pattern:

**How I solved it:**

```
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{4vY-KcK4kCIzuvzJ_jolwGUT4vJ.0FOxEzNxwyM1AzNzEzW}

```