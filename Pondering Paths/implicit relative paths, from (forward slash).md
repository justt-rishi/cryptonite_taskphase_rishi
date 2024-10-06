# implicit relative paths, from /
In this challenge we learnt about relative paths (The ones which do not start with a /). We also learnt that the current working directory does'nt matter for relative paths
(cwd is the direcotry that your prompt is currently located at). In this challenge we were required to invoke the right relative path. We were given a hint that the right 
relative path stared with a 'c', the first thought I had was why not just remove the / in /challenge/run and try it out. Crazy thing is it was the right one.
# Command Line
```
Connected!
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{oAQPT1O-JuW55oZRVFtkEZuyjhD.dlDN1QDLxcDN0czW}
```
<img width="655" alt="implicit relative paths" src="https://github.com/user-attachments/assets/81848f4f-3000-4bcd-8023-ff40cf6ed1d5">
