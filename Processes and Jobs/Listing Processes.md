# Listing Processes
In this challenge we learnt how to see all the processes that were going on in the bash at that moment using ps -ef or ps aux. In this specific challenge the main challenge
command was in a secret way, but it was alr running so we had to check all the processes that were taking place. 
## Command Line
```
Connected!
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 13:47 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init /ru
root           7       1  0 13:47 ?        00:00:00 /run/dojo/bin/sleep 6h
root          68       1  0 13:47 ?        00:00:00 /challenge/13582-run-14795
root          72      68  0 13:47 ?        00:00:00 sleep 6h
hacker        73       0  0 13:47 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        91      73  0 13:47 pts/0    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/13582-run-14795
Yahaha, you found me! Here is your flag:
pwn.college{87HyHJPWYRu_u5s7lw3KY62s_Lc.dhzM4QDLxcDN0czW}
```
<img width="848" alt="Listing Processes" src="https://github.com/user-attachments/assets/94cdc896-c1ae-4bab-8efc-4ee2092b914e">
