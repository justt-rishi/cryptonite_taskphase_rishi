# Mixing Globs
In this challenge we had to use all the previous knowledge on the concept of globbing and get only the files pwning, challenge and eductional. I got is based on trial and error.
I basically see what was affecting the output and slightly tweaked the glob to attain the flag.
## Command Line
```
Connected!
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run ?[n]*
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
incredible
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run ls c*g
Error: you called this command with more than 1 argument (pre-globbing)! Please
call me with one argument.
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run c*g
Error: you did not use a square bracket glob...
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [ce]*
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
challenging educational
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{0h0T04oMOm_WYdQP9KUh7cpSr3k.dVjM4QDLxcDN0czW}
```
<img width="668" alt="Mixed Globbing" src="https://github.com/user-attachments/assets/b508551d-7e02-4277-b0d1-f41851ac10b9">
