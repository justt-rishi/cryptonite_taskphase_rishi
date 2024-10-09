# Grepping Stored Results
In this challenge we were required to redirect the output of /challenge/run to /tmp/data.txt using >. Then we had to grep the flag from /tmp/data.txt with "pwn" in order to 
get the flag.
## Command Line
```
Connected!
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep "pwn" /tmp/data.txt
pwns
pwn
pwn.college{svPBbA_56rkcbtljyj-k_HG12gt.dhTM4QDLxcDN0czW}
pwning
pwned
```
<img width="855" alt="Grepping stored results" src="https://github.com/user-attachments/assets/97dbeaa3-4811-4b20-8378-8b1d3160fcb7">
