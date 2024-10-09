# Redirecting Errors
In this challenge we leart that we could redirect errors also into a location using File Descriptor. For example, when we use > it is basically 1> (1--->Standard output). So in 
this challenge we were required to redirect the flag into myflag and the errors into the instrcuction location. Then use the cat command to get the flag from the myflag file.
## Command Line
```
Connected!
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{ABPiuEia9TYYpHDM1DAaduFKogv.ddjN1QDLxcDN0czW}
```
<img width="620" alt="Redirecting Errors" src="https://github.com/user-attachments/assets/cef21b75-e0a1-4eb7-8671-0cc518560937">
