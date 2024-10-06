# Postion Yet Elsewhere
This agn same as the previous challenge(Position elsewhere) requires us to use the cd command to navigate to the right directory and excute the command /challenge/run to obtain
the flag. In this challenge the right directory was /proc/67 directory.
# Command Line
```
Connected!
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /proc/67 directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /proc/67
hacker@paths~position-yet-elsewhere:/proc/67$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{QEuFm6xuM2IYcQWhStqfc1uv0yC.dhDN1QDLxcDN0czW}
```
<img width="581" alt="Position Yet Elsewhere" src="https://github.com/user-attachments/assets/7f259e64-52fc-4956-a066-4e9cf575b29e">
