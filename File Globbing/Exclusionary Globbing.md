# Exlusionary Globbing
In this challenge we learnt how to file glob with the condition of not showing the files which follow the condition. Hence the name Exclusionary Globbing. In this challenge, we 
had to go to the /challenge/files directory and run /challenge/run and write a argument which doesnt start with either p,w or n.
## Command Line
```
Connected!
hacker@globbing~exclusionary-globbing:~$ /challenge/files
ssh-entrypoint: /challenge/files: Is a directory
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run file[^pwn]
Error: your argument is too long! It must be 8 characters or less.
hacker@globbing~exclusionary-globbing:/challenge/files$ ls
amazing      delightful   great       jovial    magical     pwning   splendid   victorious  youthful
beautiful    educational  happy       kind      nice        queenly  thrilling  wonderful   zesty
challenging  fantastic    incredible  laughing  optimistic  radiant  uplifting  xenial
hacker@globbing~exclusionary-globbing:/challenge/files$ ls -a
.        beautiful    educational  happy       kind      nice        queenly   thrilling   wonderful  zesty
..       challenging  fantastic    incredible  laughing  optimistic  radiant   uplifting   xenial
amazing  delightful   great        jovial      magical   pwning      splendid  victorious  youthful
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [^pwn]
Your expansion did not expand to the requested files (amazing beautiful
challenging delightful educational fantastic great happy incredible jovial kind
laughing magical optimistic queenly radiant splendid thrilling uplifting
victorious xenial youthful zesty).
Instead, it expanded to:
[^pwn]
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [^pwn]*
You got it! Here is your flag!
pwn.college{0OJ948lmqLSWMAPt5MHN6xhtzqb.dZjM4QDLxcDN0czW}
```
<img width="838" alt="Exclusionary Globbing" src="https://github.com/user-attachments/assets/8bb92b86-0ecd-487a-a07c-28f9232f5172">
