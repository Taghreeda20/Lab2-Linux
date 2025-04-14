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

6- Redirect the output of the ls command to a file called file_list.txt :      

    Taghreed20@Ubuntu5:~$ ls ~/.bashrc > file_list.txt
    
7- Use file globbing to list all .txt files in the current directory : 

    Taghreed20@Ubuntu5:~$ ls *.txt
    file_list.txt

8- Redirect the output of the ls command to a file and append it : 

    Taghreed20@Ubuntu5:~$ ls >> file1

9- Use a pipe to send the output of ls to the grep command to filter for files containing the word "report" : 

    Taghreed20@Ubuntu5:~$ ls | grep report

10- Use head to view the first 10 lines of a file, and tail to view the last 10 lines : 



        



