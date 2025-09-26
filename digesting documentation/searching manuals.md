# Searching Manuals 

**Flag:** pwn.college{k5gFSvlLAizgJcw_h5j2DLVDlM2.QX1EDO0wyM1AzNzEzW}

**What I Learnt:** You can scroll man pages with the arrow keys (and PgUp/PgDn) and search with /. After searching, you can hit n to go to the next result and N to go to the previous result. Instead of /, you can use ? to search backwards!

**How I Solved It:**
Opened The Manual and then used the / command to search for flag

```
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$
hacker@man~searching-manuals:~$ /challenge/challenge -gzobuu
Initializing...
Incorrect usage! Please read the challenge man page!
hacker@man~searching-manuals:~$ /challenge/challenge --gzobuu
Initializing...
Correct usage! Your flag: pwn.college{k5gFSvlLAizgJcw_h5j2DLVDlM2.QX1EDO0wyM1AzNzEzW}
hacker@man~searching-manuals:~$




```