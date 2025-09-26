# Helpful Programs 

**Key:**  pwn.college{E76hnnP5jubRcpBIpkhBLWW0B_Z.QX3IDO0wyM1AzNzEzW}

**What I Learnt:** Some programs don't have a man page, but might tell you how to run them if invoked with a special argument. Usually, this argument is --help 

**How I Solved It:** Used the /challenge/challenge -h command, figured out what it does, got the secret value (765) that gives you the key and got the key.

```
hacker @ manhelpful-programs:$ /challenge/challenge
No options specified.
hacker@manhelpful-programs:$ /challenge/challenge man -help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -h/--help: ignored explicit argument 'elp'
hacker@manhelpful-programs:$ /challenge/challenge -g GIVE_THE_FLAG
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: invalid int value: 'GIVE_THE_FLAG'
hacker@manhelpful-programs:$ /challenge/challenge 0g
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: unrecognized arguments: 0g
hacker@manhelpful-programs:$ /challenge/challenge -g
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: expected one argument
hacker@manhelpful-programs:$ /challenge/challenge -h
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 765
hacker@man~helpful-programs:~$ /challenge/challenge -g 765
Correct usage! Your flag: pwn.college{E76hnnP5jubRcpBIpkhBLWW0B_Z.QX3IDO0wyM1AzNzEzW}
hacker@man~helpful-programs:~$ 

```