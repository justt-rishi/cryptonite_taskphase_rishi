# Fun with Groups names
In this challenge we basically learnt how to use the id command to figure out what the name of our user was..(for this specific challenge it was not hacker rather it was 
grp24468.
## Command Line
```
Connected!
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp24468) groups=1000(grp24468)
hacker@permissions~fun-with-groups-names:~$ chgrp grp24468 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{AibBQq0lpq9jDjNxvSeEWyoAYRH.dJzNyUDLxcDN0czW}
```
<img width="559" alt="Fun with Groups Names" src="https://github.com/user-attachments/assets/479800f4-295a-472a-b348-c1ce7d81d97f">
