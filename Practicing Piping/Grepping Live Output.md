# Grepping Live Output
In this challenge we were taught how to use the | operator. It can be used to remove the "middleman" and directly grep for the file instead of coping everything into a seperate 
file and then grepping. An example is shown below:-
## Command Line
```
Connected!
hacker@piping~grepping-live-output:~$ /challenge/run | grep "pwn"
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stdout : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/xpq4yhadyhazkcsggmqd7rsgvxb3kjy4-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stdout!
[PASS] Success! You have satisfied all execution requirements.
pwn
pwns
pwning
pwned
pwn.college{wZcXFBBeYGIj1sq7IGfX_9tLmI7.dlTM4QDLxcDN0czW}
```
<img width="851" alt="Grepping Live Output" src="https://github.com/user-attachments/assets/06b70657-eaed-43a7-8f98-22407cb33ffe">
