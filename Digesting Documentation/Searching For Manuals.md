# Searching For Manuals
In this the usage of /challenge/challenge was given in a random man page. We had to search through man pages using man man and the man -k <reqfile>. And then use man to read the 
page to find out the proper usage of /challenge/challenge.
## Command Line
```
ykbkbrkvbw (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man ykbkbrkvbw

CHALLENGE(1)                                            Challenge Commands                                           CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --ykbkbr NUM
              print the flag if NUM is 436

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                                  May 2024                                                CHALLENGE(1)
hacker@man~searching-for-manuals:~$ /challenge/challenge --ykbkbr 436
Correct usage! Your flag: pwn.college{U43H6ykG1bZkbLrkvI5b0wmHyoQ.dZTM4QDLxcDN0czW}
```
<img width="696" alt="Searching For Manuals" src="https://github.com/user-attachments/assets/94ea0484-a4aa-40d7-a18f-7f6a5357c78d">
