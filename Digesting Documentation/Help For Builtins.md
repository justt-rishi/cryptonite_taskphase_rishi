# Help For Builtins
In this challenge we learnt about help builitins (basically alt for -help and man). Like the prev one we were supposed to use the secret given in the challenge to builtin to 
invoke the flag.
## Command Line
```
Connected!
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "8KJk-qQO".
hacker@man~help-for-builtins:~$ challenge --secret 8Kjk-q0
ERROR: incorrect argument to --secret. Read the help!
hacker@man~help-for-builtins:~$ challenge --secret 8KJk-qQO
Correct! Here is your flag!
pwn.college{8KJk-qQOvqiQnNMFsEAhLHDawJy.dRTM5QDLxcDN0czW}
```
<img width="595" alt="Help For Builitins" src="https://github.com/user-attachments/assets/d45b16a7-bf75-4654-9248-49a78b936fe3">
