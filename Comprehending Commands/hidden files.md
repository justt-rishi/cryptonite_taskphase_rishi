# hidden files
In this challenge I learnt about hidden files in Linux. We can access them by adding -a after ls so dub. Here we had to cat a readable file to get the flag.
## Command Line
```
root@Lucky:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@commands~hidden-files:~$ ls -a
.  ..  .ICEauthority  .bash_history  .bash_logout  .bashrc  .cache  .config  .dbus  .local  .profile  Desktop  b  leap
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-19091736328565  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat flag-19091736328565
cat: flag-19091736328565: No such file or directory
hacker@commands~hidden-files:/$ cat .flag-19091736328565
pwn.college{YEjj4AfxKGHFPnbhpW7OMNhiV6C.dBTN4QDLxcDN0czW}
```
<img width="860" alt="hidden files" src="https://github.com/user-attachments/assets/4c89b9a1-6882-40f9-a815-c7bf24e99840">
