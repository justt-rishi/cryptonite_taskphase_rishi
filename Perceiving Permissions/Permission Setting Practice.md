# Permission Setting Practice
This challenge was an extesion to the previous one. We learnt we can rewrite/overwrite permissions using the = in the argument as shown.
## Command Line
```
hacker@permissions~permissions-setting-practice:~$ chmod u=rx,g=w /challenge/pwn
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
hacker@permissions~permissions-setting-practice:~$ chmod a=rwx /flag
hacker@permissions~permissions-setting-practice:~$ cat /flag
pwn.college{YDt-sEZ2YYJ0UwfmX8Jb6NqKctn.dNTM5QDLxcDN0czW}
```
<img width="770" alt="Permission Setting Practice" src="https://github.com/user-attachments/assets/afc7839c-af00-4d4d-aa67-3dd8d069a738">
