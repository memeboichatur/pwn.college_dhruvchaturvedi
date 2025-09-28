# Writing To Multiple Programs 

**Flag:** pwn.college{k1wTEcn3sOmVQ_gSERqFIgVL52z.QXwgDN1wyM1AzNzEzW}
 
**What I learnt:** you can also use process substitution for writing to commands

**How I solved it:**


```
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) | tee >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
2153330321112017252
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{k1wTEcn3sOmVQ_gSERqFIgVL52z.QXwgDN1wyM1AzNzEzW}


```