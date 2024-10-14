# Resuming Processes
In this challenge we learnt how to use the fg bulletin to resume a suspended process. We had to run /challenge/run, suspend it and then fg to get the flag.
## Command Line
```
Connected!
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{UJ20M9ZuRs6bD99NrT_o5Gk3ZH_.dZDN4QDLxcDN0czW}
```
<img width="709" alt="Resuming Processes" src="https://github.com/user-attachments/assets/0d9e099d-89c1-42c7-87f1-11775fec32a6">
