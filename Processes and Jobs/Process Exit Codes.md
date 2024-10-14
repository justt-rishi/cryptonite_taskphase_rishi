# Process Exit Codes
In this we learnt how to get the processes exit code by using echo$? . We had to get the error code for /challenge/get-code and use it as an argument for /challenge/submit-code
to get the flag.
## Command Line
```
Connected!
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
73
hacker@processes~process-exit-codes:~$ /challenge/submit-code 73
CORRECT! Here is your flag:
pwn.college{8w0PU49sCEZhglsC7dt7fLpM3ZV.dljN4UDLxcDN0czW}
```
<img width="616" alt="Process Exit Code" src="https://github.com/user-attachments/assets/05bd5cf7-b48e-40fe-b981-7f2e8fadd9ac">
