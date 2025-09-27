# Matching Paths with []

**Flag:** pwn.college{MRTpTAV1pDqBbzictLy39V4rLky.QX0IDO0wyM1AzNzEzW}

**What I learnt:** Globbing happens on a path basis, so you can expand entire paths with your globbed arguments

**How I solved it:** 

``` 
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[absh]
You got it! Here is your flag!
pwn.college{MRTpTAV1pDqBbzictLy39V4rLky.QX0IDO0wyM1AzNzEzW}
hacker@globbing~matching-paths-with-:~$

```