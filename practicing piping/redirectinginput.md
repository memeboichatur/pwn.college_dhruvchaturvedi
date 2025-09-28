# Redirecting input

**Key:** pwn.college{cSOFo9W74fDuqPC96s4f8bX8dvq.QXwcTN0wyM1AzNzEzW}

**What I learnt:** We can redirect input using <

**How I solved it:**

```
hacker@piping~redirecting-input:~$ /challenge/run
You have not redirected anything to my standard input. Please do so, using '<'.
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{cSOFo9W74fDuqPC96s4f8bX8dvq.QXwcTN0wyM1AzNzEzW}

```

