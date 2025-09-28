# Duplicating piped data with tee

**Flag:** pwn.college{olPbxSg-vAW-mJl2U1wz3sp14EU.QXxITO0wyM1AzNzEzW}

**What I learnt:** The tee command duplicates data flowing through your pipes to any number of files provided on the command line

**How I solved it:**

first, redirected the output of /challenge/pwn to a file called pido while piping it to /challenge/college ,then read this file giving me the secret argument

```
touch pido
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee pido | /challenge/college
Processing...
WARNING: you are overwriting file pido with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat pido
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "olPbxSg-"

```

then, used this secret argument to find out the flag: 

```
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret olPbxSg- | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{olPbxSg-vAW-mJl2U1wz3sp14EU.QXxITO0wyM1AzNzEzW}

```