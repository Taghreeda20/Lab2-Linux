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
    
    Taghreed20@Ubuntu5:~$ head 10 /etc/passwd
    head: cannot open '10' for reading: No such file or directory
    ==> /etc/passwd <==
    root:x:0:0:root:/root:/bin/bash
    daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
    bin:x:2:2:bin:/bin:/usr/sbin/nologin
    sys:x:3:3:sys:/dev:/usr/sbin/nologin
    sync:x:4:65534:sync:/bin:/bin/sync
    games:x:5:60:games:/usr/games:/usr/sbin/nologin
    man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
    lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
    mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
    news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
    -------------------------------------------------------------
    Taghreed20@Ubuntu5:~$ tail 10 /etc/passwd
    tail: cannot open '10' for reading: No such file or directory
    ==> /etc/passwd <==
    cups-browsed:x:114:114::/nonexistent:/usr/sbin/nologin
    hplip:x:115:7:HPLIP system user,,,:/run/hplip:/bin/false
    gnome-remote-desktop:x:988:988:GNOME Remote Desktop:/var/lib/gnome-remote-desktop:/usr/sbin/nologin
    polkitd:x:987:987:User for polkitd:/:/usr/sbin/nologin
    rtkit:x:116:119:RealtimeKit,,,:/proc:/usr/sbin/nologin
    colord:x:117:120:colord colour management daemon,,,:/var/lib/colord:/usr/sbin/nologin
    gnome-initial-setup:x:118:65534::/run/gnome-initial-setup/:/bin/false
    nm-openvpn:x:119:121:NetworkManager OpenVPN,,,:/var/lib/openvpn/chroot:/usr/sbin/nologin
    gdm:x:120:122:Gnome Display Manager:/var/lib/gdm3:/bin/false
    Taghreed20:x:1000:1000:Taghreed20:/home/Taghreed20:/bin/bash

11- Use cut to extract the second column of a file called data.csv : 

    Taghreed20@Ubuntu5:~$ cut -d',' -f2 data.csv

12- Search for all lines in a file called log.txt that contain the word "ERROR" using grep : 

    Taghreed20@Ubuntu5:~$ grep "ERROR" log.txt

13- Create a shell variable called current_user to store the output of the whoami command : 

    Taghreed20@Ubuntu5:~$ current_user=$(whoami)
    Taghreed20@Ubuntu5:~$ echo "Current user: $current_user"
    Current user: Taghreed20

14- Use tr to convert a string of lowercase letters to uppercase : 
    
    Taghreed20@Ubuntu5:~$ echo "my name is taghreed" | tr '[:lower:]' '[:upper:]' 
    MY NAME IS TAGHREED

15- Use a pipe to send the output of ps to grep to search for a specific process name : 

    Taghreed20@Ubuntu5:~$ ps aux | grep Taghreed
    Taghree+   10457  0.0  0.0   9220  2400 pts/0    S+   21:36   0:00 grep --color=auto Taghreed

16- Create a Bash alias named ls for the command ls -l :

    Taghreed20@Ubuntu5:~$ alias ls='ls -l'

17- Use sort to sort the output of ls -l by file size : 

    Taghreed20@Ubuntu5:~$ ls -l | sort -k5 -n

18- Use grep to count the number of lines that contain the word "success" in a file : 

    Taghreed20@Ubuntu5:~$ grep -c "success" file_list.txt

19- Redirect the output of the dmesg command to a file and view the first 20 lines using head : 

    Taghreed20@Ubuntu5:~$ sudo dmesg > File.txt
    [sudo] password for Taghreed20: 
    Taghreed20@Ubuntu5:~$ head -20 File.txt

20- Use cut to extract the first field from a CSV file and display it : 

    Taghreed20@Ubuntu5:~$ cut -d',' -f1 csv








        



