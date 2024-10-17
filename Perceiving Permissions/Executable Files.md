# Executable Files
In this we just needed to give the hacker the permission to excute the /challenge/run command. I tried to do rgo+rwx but it dint work, so I had to do a+x so that anyone can
excute that command.
## Command Line
```
Connected!
hacker@permissions~executable-files:~$ chmod a+x /challenge/rin
chmod: cannot access '/challenge/rin': No such file or directory
hacker@permissions~executable-files:~$ chmod a+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{AngnKdoZE117jNHo33Sns_nxgv8.dJTM2QDLxcDN0czW}
```
<img width="793" alt="Executable Files" src="https://github.com/user-attachments/assets/80ae8516-81d6-4672-8965-5ea1f3b2ed61">
