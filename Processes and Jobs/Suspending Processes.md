# Suspending Processes
In this challenge we learnt how to suspend a process by using ctrl+z. We had to run /challenge/run suspend it and run it agn to get the flag.
## Command Line
```
Connected!
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          82      65  0 14:07 pts/0    00:00:00 bash /challenge/run
root          84      82  0 14:07 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challegne/run
ssh-entrypoint: /challegne/run: No such file or directory
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          82      65  0 14:07 pts/0    00:00:00 bash /challenge/run
root          90      65  0 14:08 pts/0    00:00:00 bash /challenge/run
root          92      90  0 14:08 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{QB40AeTmX332Ja_xO1zn5yOfBPv.dVDN4QDLxcDN0czW}
```
<img width="728" alt="Suspending Processes" src="https://github.com/user-attachments/assets/9928987e-dac0-4f28-af9f-d3b6beaf5501">
