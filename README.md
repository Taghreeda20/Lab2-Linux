# Lab2-Linux

1- List the available shells in your system : 

    Taghreed20@Ubuntu5:~$ cat /etc/shells
    # /etc/shells: valid login shells
    /bin/sh
    /usr/bin/sh
    /bin/bash
    /usr/bin/bash
    /bin/rbash
    /usr/bin/rbash
    /usr/bin/dash

2- List all of the environment variables in your current shell : 

![image](https://github.com/user-attachments/assets/7d6523ec-d51f-4efc-8c49-1b41d74a2420)

3- Display your current shell name : 

    Taghreed20@Ubuntu5:~$ echo "$shell"

4- List all of the environment variables for the Bash shell : 

![image](https://github.com/user-attachments/assets/3e909deb-01be-4391-a78a-6d409f86ce22)

5- Edit your shell profile to display the date at login and change your prompt : 

    Taghreed20@Ubuntu5:~$ sudo nano ~/.bashrc 
    echo "Today is $(date)" 

6-     
        



