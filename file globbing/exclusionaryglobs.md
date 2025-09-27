# Exclusionary Globbing

**Flag:** pwn.college{4twUqRys-KF4aXNlVJSj77-g8Oi.QX2IDO0wyM1AzNzEzW}

**What I learnt:** if we want to filter out files in a glob the [] helps you do just this. If the first character in the brackets is a ! or  a ^, the glob inverts, and that bracket instance matches characters that aren't listed.
The ! character has a different special meaning in bash when it's not the first character of a [] glob, so keep that in mind if things stop making sense! ^ does not have this problem, but is also not compatible with older shells

**How I solved it:**

```
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{4twUqRys-KF4aXNlVJSj77-g8Oi.QX2IDO0wyM1AzNzEzW}

```