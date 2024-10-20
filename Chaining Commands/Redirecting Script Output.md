# Redirecting Script Output
In this we had to do the same thing as the old challenge but then redirect it into /challenge/solve to get the flag using |.
## Command Line
```
Connected!
hacker@chaining~redirecting-script-output:~$ touch x.sh
hacker@chaining~redirecting-script-output:~$ echo "/challenge/pwn ; challenge/college" > x.sh
hacker@chaining~redirecting-script-output:~$ x.sh | /challenge/solve
ssh-entrypoint: x.sh: command not found
The data piped from /challenge/pwn did not match what I expected. I
re-randomize the data every time you input a new line to the shell, so you must
get it right in one shot! Make sure to pipe the output from your script to
/challenge/solve.
hacker@chaining~redirecting-script-output:~$ x.sh > /challenge/solve
ssh-entrypoint: /challenge/solve: Permission denied
hacker@chaining~redirecting-script-output:~$ (/challenge/pwn; /challenge/college) | /challenge/solve
Correct! Here is your flag:
pwn.college{YeYv6vtsdIsNulMVLTSbsZxaA5Z.dhTM5QDLxcDN0czW}
```
<img width="748" alt="Redirecting Script Output" src="https://github.com/user-attachments/assets/7a91605b-9270-4cce-9448-c64dec7df393">
