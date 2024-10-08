# Reading Manuals
This challenge teaches us about the man command which is used to learn more about a command or function. For example to get the flag we had to use the man command to know how to
use the challenge command in the right way to get the flag.
# Command Line
```
Connected!
hacker@man~reading-manuals:~$ man challenge

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

       --wyevhp NUM
              print the flag if NUM is 816

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                                  May 2024                                                CHALLENGE(1)
hacker@man~reading-manuals:~$ /challenge/challenge
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ challenge --wyevhp 816
ssh-entrypoint: challenge: command not found
hacker@man~reading-manuals:~$ /challenge/challenge --wyevhp 816
Correct usage! Your flag: pwn.college{wUAy8S1X-UOevXNhKRpbQ6L0TNV.dRTM4QDLxcDN0czW}
```
<img width="605" alt="Reading manuals" src="https://github.com/user-attachments/assets/3a066725-80fd-45cf-b811-a567a1306f38">
