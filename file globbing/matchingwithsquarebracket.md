# Matching with []

**Flag:** pwn.college{Yb2XnuJDgQPZC5s_kKTw1XCK5t2.QXzIDO0wyM1AzNzEzW}

**What I learnt:** The square brackets are, essentially, a limited form of ?, in that instead of matching any character, [] is a wildcard for some subset of potential characters, specified within the brackets.
 
**How I solved it:**

```
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[abhs]
You got it! Here is your flag!
pwn.college{Yb2XnuJDgQPZC5s_kKTw1XCK5t2.QXzIDO0wyM1AzNzEzW}
hacker@globbing~matching-with-:/challenge/files$

```
