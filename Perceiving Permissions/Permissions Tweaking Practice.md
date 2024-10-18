# Permissions Tweaking Practice
In this challenge we got more practice on the chmod command. We had to use the chmod properly on /challenge/pwn to get permission to use chmod on /flag. 
## Command Line
```
hacker@permissions~permission-tweaking-practice:~$ chmod g+x /challenge/pwn
You set the correct permissions!
You've solved all 8 rounds! I have changed the ownership
of the /flag file so that you can 'chmod' it. You won't be able to read
it until you make it readable with chmod!

Current permissions of "/flag": ---------
- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod a+rwx /flag
hacker@permissions~permission-tweaking-practice:~$ cat /flag
pwn.college{c0U9pwyB4xTzQhTxi4xrhfqdXKt.dBTM2QDLxcDN0czW}
```
<img width="836" alt="Permission Tweaking Practice" src="https://github.com/user-attachments/assets/25bfd9a3-de89-4707-af01-f73f06e3ae9b">
