# Helpful Programs
This challenge we were taught about the --help command which could be used as an alternative for man command if a function doesnt have a man page. Here in this challege we were 
supposed to use the --help command to get a secret value (397) which can be used with the /challenge/challenge -g to get the flag. 
## Command Line
```
Connected!
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/chalenge -g
ssh-entrypoint: /challenge/chalenge: No such file or directory
hacker@man~helpful-programs:~$ /challenge/challenge --give-the-flag
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: expected one argument
hacker@man~helpful-programs:~$ /challenge/challenge --give-the-flag GIVE_THE_FLAG
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: invalid int value: 'GIVE_THE_FLAG'
hacker@man~helpful-programs:~$ --help
ssh-entrypoint: --help: command not found
hacker@man~helpful-programs:~$ /challenge --help
ssh-entrypoint: /challenge: Is a directory
hacker@man~helpful-programs:~$ /challenge/challenge --print-value
The secret value is: 397
hacker@man~helpful-programs:~$ /challenge/challenge -g 397
Correct usage! Your flag: pwn.college{cRqIBc39EyzKn7rAx73U7Mn-6GL.ddjM4QDLxcDN0czW}
```
<img width="772" alt="Helpful Programs" src="https://github.com/user-attachments/assets/2152f951-8e7a-47e8-9618-64856e13f32d">
