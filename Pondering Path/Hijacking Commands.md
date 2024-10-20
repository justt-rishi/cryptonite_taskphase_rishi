# Hijacking Commands
This is the same as the previous challenge. Here we had to trick it into using the fake rm command we made which has the cat /flag command in it. Then it will invoke the false
rm and then give us the flag.
## Command Line
```
Connected!
hacker@path~hijacking-commands:~$ nano
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ ls -l rm
-rwxr-xr-x 1 hacker hacker 24 Oct 20 17:03 rm
hacker@path~hijacking-commands:~$ export PATH="$HOME:$PATH"
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
Found 'rm' command at /home/hacker/rm. Executing!
pwn.college{YvWBS7i9tg1o2jk265OY7pvCUhB.ddzNyUDLxcDN0czW}
```
![Uploading Hijacking Commands.png…]()
