# Storing Command Output
In this challenge I leart that we can store the output of a command in a variable by using the $ sign infront of the command. In this challenge we had to store the output of
/challenge/run in PWN variable and get the flag using echo $PWN.
## Command Line
```
Connected!
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo PWN
PWN
hacker@variables~storing-command-output:~$ cat PWN
COLLEGE
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{MdKTnx_56E1XvFudI1V2_F3VNCK.dVzN0UDLxcDN0czW}
```
<img width="642" alt="Storing Command Output" src="https://github.com/user-attachments/assets/e1c9eefa-262c-40f9-b0d0-cd770faa7935">
