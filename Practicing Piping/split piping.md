# Split piping stderr and stdout
In this challenge we were required to use all our knowledge on piping to redirect out stderr and stdout to the required locations without them mixing up. 
I achieved this with /challenge/hack > >( /challenge/planet ) 2> >( /challenge/the ).
1) /challenge/hack: This is the command that generates both stdout and stderr.
2) '>' : This operator is used to redirect stdout.
3) '> ( /challenge/planet )': This uses process substitution to redirect stdout to /challenge/planet.
4) 2> : This operator is used to redirect stderr.
5) '> ( /challenge/the )': This redirects stderr to /challenge/the using process substitution.
This was really hard to achieve and took a lot of time..but I got it by going thru all the methods once again and brainstorming ways.
## Command Line
```
Connected!
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >( /challenge/planet ) 2> >( /challenge/the )
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{o8AoBFetaNdOuVz3RiVNIIt1olA.dFDNwYDLxcDN0czW}
```
<img width="856" alt="Split Piping" src="https://github.com/user-attachments/assets/574ef1c9-9161-4799-bbac-484cc02b8644">
