# Matching with *
In this challenge we learnt how to use * in an argument. We learnt the when shell encounter the * character it treats it as a Wildcard and do all the things with the match. 
For example, U can change directory to /challenge with out actually typing out the whole thing like shown below.
## Command Line
```
Connected!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /challenge*
You specified the path to 'cd' to in more than 4 characters. Disallowed!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /chal*
You specified the path to 'cd' to in more than 4 characters. Disallowed!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{cpSHgmf4x42TmgMRBCRKIIL0CSN.dFjM4QDLxcDN0czW}
```
<img width="635" alt="Matching with star" src="https://github.com/user-attachments/assets/fad25d1c-bcf2-43c8-b44f-64fa15bd3d7c">
