# Reading Input

**Flag:** pwn.college{E61Z-xHyKnbTHsOrlixLGScxfsR.QX4cTN0wyM1AzNzEzW}


**What I learnt:** read reads input into a variable
can also add the -p command to print out text before getting the input as : read -p "<your text here>" <var name>

**How I solved it:**

```
read -p "INPUT: " PWN
INPUT: COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{E61Z-xHyKnbTHsOrlixLGScxfsR.QX4cTN0wyM1AzNzEzW}

```