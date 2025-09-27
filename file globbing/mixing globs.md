# Mixing Globs 

**Flag:** pwn.college{88PHRB7EzLN1_T1zHNyOGh-teLh.QX1IDO0wyM1AzNzEzW}

**What I learnt:** revision of previous levels.

**How I solved it:**
navigated to /challenge/files ,listed all files to see how I could narrow down into something the three have in common, then used the command /challenge/run [cep]* which looked for the first character to start from c e or p and then anything else. this gave me my flag. the following code was used:

``` 
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{88PHRB7EzLN1_T1zHNyOGh-teLh.QX1IDO0wyM1AzNzEzW}
hacker@globbing~mixing-globs:/challenge/files$
```