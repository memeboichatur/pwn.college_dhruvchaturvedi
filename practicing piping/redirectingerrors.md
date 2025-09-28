# Redirecting Errors

**Flag:** pwn.college{IcGmnkIUj0CWuuLVKS9Hyb09bW0.QX3YTN0wyM1AzNzEzW}

**What I learnt:** A File Descriptor (FD) is a number that describes a communication channel in Linux
FD 0: Standard Input
FD 1: Standard Output
FD 2: Standard Error
When you redirect process communication, you do it by FD number
some FD numbers are implicit, eg echo hi > abc is equivalent to hi 1> abc
Furthermore, you can redirect multiple file descriptors at the same time!

**How I solved it:**

```
hacker@piping~redirecting-errors:~$ /challenge/run 1> myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat instructions
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will check that error output is redirected to a specific file path : instructions
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!

[TEST] You should have redirected my stderr to instructions. Checking...

[PASS] The file at the other end of my stderr looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{IcGmnkIUj0CWuuLVKS9Hyb09bW0.QX3YTN0wyM1AzNzEzW}


```