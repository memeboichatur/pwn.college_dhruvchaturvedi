# Grepping Live Output

**Flag:** pwn.college{oD2MwAbS4sduqUI44E7axg2Bvhx.QX5EDO0wyM1AzNzEzW}

**What I learnt:** we can avoid the need to store results to a file, using the | operator (called pipe operator) standard output from the command to the left of the pipe will be connected to (piped into) the standard input of the command to the right of the pipe.

**How I solved it:** ran the command /challenge/run | grep pwn, giving me the flag 

```
hacker@piping~grepping-live-output:~$ /challenge/run | grep pwn
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stdout : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stdout!
[PASS] Success! You have satisfied all execution requirements.
pwn
pwning
pwns
pwned
pwn.college{oD2MwAbS4sduqUI44E7axg2Bvhx.QX5EDO0wyM1AzNzEzW}

```