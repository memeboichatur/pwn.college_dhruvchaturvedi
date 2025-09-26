# Help For BuiltIns

**Flag:** pwn.college{wnnE1zHGWySBsJdc70KGvyR9FU6.QX0ETO0wyM1AzNzEzW}

**What I learnt:** Some commands, rather than being programs with man pages and help options, are built into the shell itself. These are called builtins. Builtins are invoked just like commands, but the shell handles them internally instead of launching other programs


**How I Solved it:**

Used the help challenge command to learn about the command, and then using the secret key got the flag.

``` hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "wnnE1zHG".
hacker@man~help-for-builtins:~$ challenge --secret wnnE1zHG
Correct! Here is your flag!
pwn.college{wnnE1zHGWySBsJdc70KGvyR9FU6.QX0ETO0wyM1AzNzEzW}

hacker@man~help-for-builtins:~$

```