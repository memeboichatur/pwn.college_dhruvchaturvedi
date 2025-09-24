key:pwn.college{8pmUn33PZAjoW4ItMhAnoP5_Slf.QX5ETN1wyM1AzNzEzW}

what I learnt: we can use the ls -ld command to get further information on the type of file
links are of two types- hard links and soft links

hard links are an alternative path to the same file.
soft links when accessed point the address of where the real file is. we commonly use soft links.
soft links are also called symbolic links.

they are accessed by ln -s <original file> <link location>


how I solved it:
wasn't able to figure out what to do, asked a friend who told me I could remove files(I didn't know removing files could be allowed in this challenge, will keep this in mind from now)

I removed the old not the flag by the link file, giving me access to the key.
