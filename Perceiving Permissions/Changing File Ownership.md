# Changing File Ownership
We learnt how to change the ownership of a file from one user to an other using the chown command. We have to note that this command can be used only if we are the root user, 
but for this challenge specifically we were allowed to use the command even as the hacker user. We had to change the ownership of the /flag file and cat /flag to get the flag.
## Command Line
```
Connected!
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{I-eS7roVddXS57NkkhNcCIoboRD.dFTM2QDLxcDN0czW}
```
<img width="572" alt="Changing File Ownership" src="https://github.com/user-attachments/assets/12cf463f-e926-4ba7-a2bc-f333fbd5d99b">
