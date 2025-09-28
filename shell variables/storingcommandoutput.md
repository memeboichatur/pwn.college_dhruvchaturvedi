# Storing Command Output

**Flag:** pwn.college{MS67vsJRL0j_44tc2nepoH8esR0.QX1cDN1wyM1AzNzEzW}

**What I learnt:** <var>=$(<command>) can store the output of said command into the variable. This is called command substitution. 

**How I solved it:**

```
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo "$PWN"
pwn.college{MS67vsJRL0j_44tc2nepoH8esR0.QX1cDN1wyM1AzNzEzW}

```