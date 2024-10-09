# Duplicating Piped Data with tee
In this challenge we learnt how to use the tee command to intercept a piping. This command gives a duplicate file of what is being piped. In the challenge we were required to 
read the piping by duplicating it into a text file which had the secret usage to get the flag. Below is how it is done:-
## Command Line
```
Connected!
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee output.txt | /challenge/college
Processing...
WARNING: you are overwriting file output.txt with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat output.txt
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "IIArozkd"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret IIArozkd | /challenge/cillege
ssh-entrypoint: /challenge/cillege: No such file or directory
Processing...
^[[AYou must pipe the output of /challenge/pwn into /challenge/college (or 'tee'
for debugging).
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret IIArozkd | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{IIArozkduadFtsPTkys6tthH2f9.dFjM5QDLxcDN0czW}
```
<img width="749" alt="Duplication piped stuff using tee" src="https://github.com/user-attachments/assets/cabc0de2-2049-4382-97a5-e1971553b768">
