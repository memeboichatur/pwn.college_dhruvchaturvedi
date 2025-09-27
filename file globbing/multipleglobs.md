# Multiple Globs

**Flag:** pwn.college{s7qeHfgd8w0PjbCog6lNB_NssUE.0lM3kjNxwyM1AzNzEzW}

**What I learnt:** Bash supports the expansion of multiple globs in a single word

**How I solved it:**

```
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{s7qeHfgd8w0PjbCog6lNB_NssUE.0lM3kjNxwyM1AzNzEzW}
hacker@globbing~multiple-globs:/challenge/files$


```