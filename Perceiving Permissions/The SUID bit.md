# The SUID Bit
In this we learnt how to add the suid bit to the permissions which allows us to open a new shell as the root user. From there we can just cat the /flag file.
## Command Line
```
Connected!
hacker@permissions~the-suid-bit:~$ chmod a+rws /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{sdc-WLz_Lng8cNI4e2isq_GaCBI.dNTM2QDLxcDN0czW}
```
![Uploading The SUID Bit.png…]()
