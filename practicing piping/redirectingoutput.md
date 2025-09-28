# Redirecting Output

**Flag:** pwn.college{ITFsWD-7MEadbL92hb5pZLoJwkD.QX0YTN0wyM1AzNzEzW}

**What I learnt:**

Standard Input is the channel through which the process takes input. For example, your shell uses Standard Input to read the commands that you input.
Standard Output is the channel through which processes output normal data, such as the flag when it is printed to you in previous challenges or the output of utilities such as ls.
Standard Error is the channel through which processes output error details. For example, if you mistype a command, the shell will output, over standard error, that this command does not exist.

Because these three channels are used so frequently in Linux, they are known by shorter names: stdin, stdout, stderr.

output redirection: we can redirect stdout to files using > character using echo hi > asdf


**How I solved it:** 
typed the following 

```
hacker@piping~redirecting-output:~$ echo PWN > COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your
flag:
pwn.college{ITFsWD-7MEadbL92hb5pZLoJwkD.QX0YTN0wyM1AzNzEzW}
```