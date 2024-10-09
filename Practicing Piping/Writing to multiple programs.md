# Writning to multiple programs
In this challenge we were required to use all the knowledge we know and were given to duplicate /challenge/hack output as input to both the /challenge/the and the 
/challenge/planet commands. This can be done by running /challenge/hack | tee >( /challenge/the ) >( /challenge/planet ).
## Command Line
```
root@Lucky:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >( /challenge/the ) >( /challenge/planet )
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
9687202583015015622
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{AmJ5tK3YlXV_Xbq3P0yOXDf7OLv.dBDO0UDLxcDN0czW}
```
<img width="800" alt="writing to multiple programs" src="https://github.com/user-attachments/assets/6b9dfade-ced8-4d52-962e-50e4a751af53">
