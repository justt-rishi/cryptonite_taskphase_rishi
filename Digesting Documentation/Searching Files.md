# Searching Files
In this challenge we learnt how to use the / in man command to find the required argumenat for a certain function or command. We also learnt the n is to go to next result and N
is to go to the prev result.
# Command Line
```
Connected!
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge -khe /flag
Initializing...
Incorrect usage! Please read the challenge man page!
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ challenge -khe /flag
ssh-entrypoint: challenge: command not found
hacker@man~searching-manuals:~$ /challenge/challenge --khe /flag
Initializing...
Correct usage! Your flag: pwn.college{wJgnWlgO2O5Px54Eq2Dua3O4Le8.dVTM4QDLxcDN0czW}
```
<img width="619" alt="Searching For Manuals" src="https://github.com/user-attachments/assets/c3ed69d1-b692-4d70-ab4b-dc525c482d17">
