# Killing Processes
In this challenge we learnt how to kill a processes using the kill [PID] command. So there is this process /challenge/dont_run running which doesnt let the /challenge/run run.
We had to terminate dont_run for the /challenge/run to run. 
## Command Line
```
Connected!
hacker@processes~killing-processes:~$ ps -e | grep /challenge/dont_run
hacker@processes~killing-processes:~$ cd /challenge
hacker@processes~killing-processes:/challenge$ ps -e | grep dont_run
hacker@processes~killing-processes:/challenge$ /run
ssh-entrypoint: /run: Is a directory
hacker@processes~killing-processes:/challenge$ cd
hacker@processes~killing-processes:~$ /challenge/run
Nope! /challenge/dont_run is still running! You gotta terminate it before I
give you the flag!
hacker@processes~killing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 13:55 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init /ru
root           7       1  0 13:55 ?        00:00:00 /run/dojo/bin/sleep 6h
root          71       1  0 13:55 ?        00:00:00 su -c /challenge/.launcher hacker
hacker        73      71  0 13:55 ?        00:00:00 /challenge/dont_run
hacker        74      73  0 13:55 ?        00:00:00 sleep 6h
hacker        75       0  0 13:55 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker       101      75  0 13:58 pts/0    00:00:00 ps -ef
hacker@processes~killing-processes:~$ cd /challenge
hacker@processes~killing-processes:/challenge$ ps -ef | grep dont_run
hacker        73      71  0 13:55 ?        00:00:00 /challenge/dont_run
hacker       103      75  0 13:58 pts/0    00:00:00 grep --color=auto dont_run
hacker@processes~killing-processes:/challenge$ kill dont_run
ssh-entrypoint: kill: dont_run: arguments must be process or job IDs
hacker@processes~killing-processes:/challenge$ kill 73
hacker@processes~killing-processes:/challenge$ /run
ssh-entrypoint: /run: Is a directory
hacker@processes~killing-processes:/challenge$ cd
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{kN_V0O8pJFQC9le4_Ac1J1Hf-WN.dJDN4QDLxcDN0czW}
```
<img width="851" alt="Killing Processes" src="https://github.com/user-attachments/assets/611f28d7-3ab9-4131-9044-d1a5e8aa0655">
