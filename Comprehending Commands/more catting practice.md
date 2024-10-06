# more catting practice 
In this challenge we got more exposure to the cat command in bash. We were not allowed to use the cd command so we had to use absolute path arguments to get the flag. Here the
absolute path was /lib/x86_64-linux-gnu/perl-base/flag. (I happen to not read the intial message properly and got the right path in a weird way oops)
## Command Line
```
Connected!
You cannot use the 'cd' command in this level, and must retrieve the flag by
absolute path. Plus, I hid the flag in a different directory! You can find it
in the file /lib/x86_64-linux-gnu/perl-base/flag. Go cat it out **without**
cding into that directory!
hacker@commands~more-catting-practice:~$ cat flag
cat: flag: No such file or directory
hacker@commands~more-catting-practice:~$ cat /flag
cat: /flag: No such file or directory
hacker@commands~more-catting-practice:~$ cd /
You used 'cd'! In this level, I don't allow you to change the working directory
--- you MUST chase pass 'cat' the absolute path of where I put it on the
filesystem (which is /lib/x86_64-linux-gnu/perl-base/flag).
hacker@commands~more-catting-practice:~$ cat /lib/x86_64-linux-gnu/perl-base/flag
pwn.college{4gSyssLa3LZozNa7NxJcaNdWkFn.dBjM5QDLxcDN0czW}
```
<img width="644" alt="more catting practice" src="https://github.com/user-attachments/assets/82fc832f-3bca-4c75-86e7-9051d99deeac">
