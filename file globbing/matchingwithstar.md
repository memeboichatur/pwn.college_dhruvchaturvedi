# Matching with *

**Flag:** pwn.college{AS-Vyb8gbYdjX8N9JQ0epE_iqED.QXxIDO0wyM1AzNzEzW}

**What I Learnt:** 

Globbing lets you reference files without typing them all out, or typing out their full paths
When it encounters a * character in any argument, the shell will treat it as a "wildcard" and try to replace that argument with any files that match the pattern
When zero files are matched, by default, the shell leaves the glob unchanged:

Basically, the * command works like an autofill, completing file names etc for you.

**How I solved it:**

Typed the following: 

```
hacker@globbing~matching-with-:/challenge$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{AS-Vyb8gbYdjX8N9JQ0epE_iqED.QXxIDO0wyM1AzNzEzW}
hacker@globbing~matching-with-:/challenge$


```