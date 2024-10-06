# implicit relative path
This was the same as the previous challenges. It taught me how to use the '.'. This prevents us accidentally excute programs in the home directory. We have to tell linux to run
/excute by using the '.'.
## Command Line
```
Connected!
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./challenge/run
ssh-entrypoint: ./challenge/run: No such file or directory
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{o6fJr-5gDh6etI8_S_NWgqCjG4i.dFTN1QDLxcDN0czW}
```
<img width="500" alt="implicit relative paths_1" src="https://github.com/user-attachments/assets/446ebd6d-fe0f-4480-8e99-a5052a0083c2">
