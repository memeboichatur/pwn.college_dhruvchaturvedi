# Exporting Variables

**Flag:** pwn.college{8zuMowugOv3EZR1_bdKwPKjeQl2.QXyYTN0wyM1AzNzEzW}

**What I learnt:** By default, variables that you set in a shell session are local to that shell process.
When you export your variables, they are passed into the environment variables of child processes

**How I solved it:**

```
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{8zuMowugOv3EZR1_bdKwPKjeQl2.QXyYTN0wyM1AzNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!

```