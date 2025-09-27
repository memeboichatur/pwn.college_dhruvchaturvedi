# Matching with ?

**Flag:** pwn.college{EBKFepfkkyx3fGqVnB6V4gKv50d.QXyIDO0wyM1AzNzEzW}

**What I learnt:** the ? works like *, but only matches one character. To add multiple characters, use multiple question marks.
 
**How I solved it:** 

Typed the following command: 

```
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{EBKFepfkkyx3fGqVnB6V4gKv50d.QXyIDO0wyM1AzNzEzW}
hacker@globbing~matching-with-:/challenge$


```