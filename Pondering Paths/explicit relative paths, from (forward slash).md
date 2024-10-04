# explicit relative paths, from /
In this challenge we learnt that every directory had two implicit entries that you can referance in paths: . and .. The first refers straight to the same direcotry so we can use
it make identical absolute paths for example,
/do
/./do
/do/. etc etc are all the same.
In this challenge we were asked to use the . in our relative paths to get the flag. 
```
Connected!
hacker@paths~explicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{w0jM4EOImzclxuYLdPLnjO8cBqe.dBTN1QDLxcDN0czW}
```
<img width="629" alt="explicit relative paths" src="https://github.com/user-attachments/assets/5e36e370-cf22-4793-9d5a-617de3538dcc">
