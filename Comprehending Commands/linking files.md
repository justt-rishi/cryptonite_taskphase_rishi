# Linking Files
In this challenge we learnt how to link files. We learnt about hard link and soft link and also that soft link is more used. The command for it is ln -s. I had a error with 
the /home/hacker/not-the-flag already existing, so i had to ln -sf to overwrite and then i had to simply run /challenge/catflag.
## Command Line
```
root@Lucky:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
ln: failed to create symbolic link '/home/hacker/not-the-flag': File exists
hacker@commands~linking-files:~$ cd /home/hacker
hacker@commands~linking-files:~$ touch not-the-flag1
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag1
ln: failed to create symbolic link '/home/hacker/not-the-flag1': File exists
hacker@commands~linking-files:~$ ln -sf /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ cat /challenge/catflag
#!/opt/pwn.college/bash

fold -s <<< "About to read out the /home/hacker/not-the-flag file!"
cat /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{cjU5r6oPD_87PoSvABi8AKl-0rO.dlTM1UDLxcDN0czW}
```
<img width="677" alt="Linking Files" src="https://github.com/user-attachments/assets/f11ab30f-ee29-4727-a1cc-e601e47ae14d">
