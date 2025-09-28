# Printing Exported Variables

**Flag:** pwn.college{otZOC81rzo2FF_CT72x9XkUkCvJ.QX4UTN0wyM1AzNzEzW}

**What I learnt:** learnt what the env command does (print out every exported variable set in your shell)

**How I solved it:**

```
hacker@variables~printing-exported-variables:~$ env | grep FLAG
FLAG=pwn.college{otZOC81rzo2FF_CT72x9XkUkCvJ.QX4UTN0wyM1AzNzEzW}

```