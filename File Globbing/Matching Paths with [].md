# Matching Paths with []
This is a more adv usage of the bracket-globbing. It directly uses the brackets in paths...so we dont need to change the directory before running.
## Command Line
```
Connected!
hacker@globbing~matching-paths-with-:~$ /challenge.run
ssh-entrypoint: /challenge.run: No such file or directory
hacker@globbing~matching-paths-with-:~$ /challenge/run
Error: you did not use a square bracket glob...
hacker@globbing~matching-paths-with-:~$ /challenge/run file_[bash]
Error: you will need to specify the path to the files as part of your glob
argument, since they are in a different directory than your current working
directory!
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files file_[bash]
Error: you called this command with more than 1 argument (pre-globbing)! Please
call me with one argument.
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{o7ZlVgYeD0RoxoX4VKTwUchZXA_.dRjM4QDLxcDN0czW}
```
<img width="692" alt="matching path with sq bracket" src="https://github.com/user-attachments/assets/c01da9c2-1710-43f8-b016-8e167faa9a7e">
