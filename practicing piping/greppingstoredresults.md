# Grepping Stored Results

**Flag:** pwn.college{8fwMmsGT2MpxjlOy1NsKyHC9mI-.QX4EDO0wyM1AzNzEzW}

**What I Learnt:** n/a 

**How I Solved it:**

```
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep flag /tmp/data.txt
[FLAG] Here is your flag:
flagrant
camouflage's
flagstaff
flagpoles
camouflaged
camouflages
flagellation's
flagellums
conflagration's
camouflaging
conflagration
flagstone's
flagrantly
flagging
unflagging
flagella
flagships
flagship
persiflage
flagpole's
flagstaffs
flagstaff's
flagship's
persiflage's
flagellating
flagstones
flagon
flagellum's
flags
flagellates
flagellated
flagon's
flagged
camouflage
flag
flagons
flagpole
flag's
conflagrations
flagellation
flagstone
flagellum
flagellate
hacker@piping~grepping-stored-results:~$ grep pwn /tmp/data.txt
pwned
pwn
pwns
pwn.college{8fwMmsGT2MpxjlOy1NsKyHC9mI-.QX4EDO0wyM1AzNzEzW}
pwning

```