# Other users with su
In this we had to switch to a specific user 'zardus' (not the root user). We had to this by giving zardus as an argument to the su command. Then we had to run the /challenge/run
command to get the flag.
## Command Line
```
Connected!
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ cat /flag
cat: /flag: Permission denied
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{4DgWGb38jsNVFhm9F2BsreFVBls.dZTN0UDLxcDN0czW}
```
<img width="533" alt="Other users with su" src="https://github.com/user-attachments/assets/af4bc022-4af9-48b4-a751-8daf9b9430b4">
