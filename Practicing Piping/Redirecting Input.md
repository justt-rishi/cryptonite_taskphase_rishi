# Redirecting Input
In this challege we were taught how to use <.....which is use to redirect input to a location. In this challenge we were required to set redirect COLLEGE in PWN using the < 
charecter and the echo command. After this we were supposed to use the < in /challenge/run and use the PWN as input to get the flag.
## Command Line
```
Connected!
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ echo pwn
pwn
hacker@piping~redirecting-input:~$ cat pwn
cat: pwn: No such file or directory
hacker@piping~redirecting-input:~$ cat PWN
COLLEGE
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{YlTxtgUvn_8Kr0vsJUSod_uCO30.dBzN1QDLxcDN0czW}
```
<img width="638" alt="Redirecting Input" src="https://github.com/user-attachments/assets/d12da805-b811-4c87-8d28-56f5b7f66ef6">
