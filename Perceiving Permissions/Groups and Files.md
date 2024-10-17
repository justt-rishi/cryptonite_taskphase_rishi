# Groups and Files
In this one we learnt how to instead of changing the ownership of a file, how we can rather add the file grp directly to the hacker user. We can do this by using the chgrp
command which changes the user to the desired grp like shown below.
## Command Line
```
Connected!
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /falg
cat: /falg: No such file or directory
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{EocI9QufabTCrYkv2kBUUJBvE5X.dFzNyUDLxcDN0czW}
```
<img width="532" alt="Groups and Files" src="https://github.com/user-attachments/assets/0e9844ef-c2fb-45ea-9e73-1feca2dd7e7d">
