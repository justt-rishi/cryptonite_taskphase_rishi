# Grepping Errors
In this challenge we learnt that we cant use | for errors (fd 2) cuz it is only defined for standard output (fd 1). So we learnt that there is a operator to help with that which
is 2>&1. It bascially does the 2 step process of moving the error into output and then pipe the now combined thing to directly use the | operator as shown below.
## Command Line
```
Connected!
hacker@piping~grepping-errors:~$ /challenge/run 2>&1 | grep "pwn"
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/xpq4yhadyhazkcsggmqd7rsgvxb3kjy4-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwn
pwning
pwned
pwns
pwn.college{s2_852B2lsl5vNNbc5c3wxYIlGy.dVDM5QDLxcDN0czW}
hacker@piping~grepping-errors:~$
```
<img width="860" alt="Grepping Errors" src="https://github.com/user-attachments/assets/d8da3342-34fe-466a-864f-96c3dde3fe3f">
