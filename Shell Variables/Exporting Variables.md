# Exporting Variables
In this challenge, we mostly learned how to export variables using the export command. We also learned a little about the sh command which opens a baby shell within the main shell.
In this challenge, we had to export PWN=COLLEGE and not export COLLEGE=PWN and run the /challenge/run command to get the flag.
## Command Line
```
Connected!
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{4OHXigSM3v_K4SPuHf6JAg9u5uU.dJjN1QDLxcDN0czW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$
```
<img width="646" alt="Exporting Variables" src="https://github.com/user-attachments/assets/23d9303a-829f-464e-bbee-0e6fd8978a03">
