# Process Substitution for Input

**Flag:** pwn.college{QnSQUGcCBHjmQY3aFfLNii6xrml.0lNwMDOxwyM1AzNzEzW}

**What I learnt:** We can hook input and output of programs to arguments of commands. This is done using Process Substitution.
use <(arg here) to do so

**How I solved it:**

```
 diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
10a11
> pwn.college{QnSQUGcCBHjmQY3aFfLNii6xrml.0lNwMDOxwyM1AzNzEzW}

```