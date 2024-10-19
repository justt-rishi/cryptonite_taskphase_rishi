# Cracking Passwords
In this we learnt that the password for the su command can be cracked, as they are generally stored in /etc/shadow. Here we had to crack the password for zardus by cding to 
/challenge and then checking the leaked file provided in the story. Then it was same old same old.
## Command Line
```
Connected!
hacker@users~cracking-passwords:~$ john shadow-leak
Created directory: /home/hacker/.john
stat: shadow-leak: No such file or directory
hacker@users~cracking-passwords:~$ john ./my-leaked-shadow-file
stat: ./my-leaked-shadow-file: No such file or directory
hacker@users~cracking-passwords:~$ cd /challenge
hacker@users~cracking-passwords:/challenge$ john ./my-leaked-shadow-file
stat: ./my-leaked-shadow-file: No such file or directory
hacker@users~cracking-passwords:/challenge$ john shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:08 85% 1/3 0g/s 280.2p/s 280.2c/s 280.2C/s Zardus1111..z99999123456
0g 0:00:00:16 0% 2/3 0g/s 279.9p/s 279.9c/s 279.9C/s keller..nation
0g 0:00:00:18 1% 2/3 0g/s 281.6p/s 281.6c/s 281.6C/s katrina..karla
0g 0:00:00:20 1% 2/3 0g/s 282.8p/s 282.8c/s 282.8C/s Johnson..buzz
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04766g/s 277.5p/s 277.5c/s 277.5C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:/challenge$ su zardus
Password:
zardus@users~cracking-passwords:/challenge$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{kg3Zu0pF_mlwvzclsptF4eVuk0P.ddTN0UDLxcDN0czW}
```
<img width="734" alt="Cracking Passwords" src="https://github.com/user-attachments/assets/cbafb5f3-cea6-4f73-96a6-eddd9109a9e6">
