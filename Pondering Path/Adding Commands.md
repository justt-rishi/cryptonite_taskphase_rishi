# Adding Commands 
In this we learnt how to add commands to the PATH file. We had create a shell script called win which had the cat /flag commands in it. Then we had to export the win command to
the PATH. Then we had to run the /challenge/run directory to get the flag. This challenge was such a pain in the ass.....I had to use the help of the inbuilt AI in the help 
section to get the flag. (It was fun tho....the confusion and all)
## Command Line
```
hacker@path~adding-commands:~$ cd /home/hacker
hacker@path~adding-commands:~$ nano win
hacker@path~adding-commands:~$ chmod +x win
hacker@path~adding-commands:~$ export PATH="$HOME:$PATH"
hacker@path~adding-commands:~$ echo $PATH
/home/hacker:/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{oSkYUTTbHU43S-RRiR2OItQfkJQ.dZzNyUDLxcDN0czW}
```
<img width="821" alt="Adding Command" src="https://github.com/user-attachments/assets/4c0ccfb2-afa9-4066-9d65-dbe54f72b363">
