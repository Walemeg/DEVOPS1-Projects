# Linux Practice Project

## Goal and Pre-requisite

The goal of this project is to refine my Linux skill; gain hands-on experience and develop a solid foundation. The report below contains 40 Linux commands.

For the purpose of this practice, I will be using linux teminal on GitBash. I connected to EC2 instance with IP address 172-31-34-148 

### 1) Sudo Commands
"super user do" and it allows you to temporarily elevate your current user account to have root privileges.

'Sudo apt upgrade'

![](Images/Sudo%20apt%20upgrade.PNG)

### 2) pwd Commands
PWD means Present Working Directory and shows current folder I ma currently working in

### 3) cd Commands
CD it means Change Directory and used for moving from one folder to the other

Note : Below is the out put for practice '2' and '3'.
I created a folder inside Ubuntu folder called Commandsline and also created a folder called unixcommamds inside commandsline folder
pwd commands showed the initail directory, I used CD to commandsline directory and applied 'pwd' command again.
I used "cd .." and "cd -" to move to the previous directory and next directory repectively as shown below

![](Images/PWD%20&%20CD%20command.PNG)

### 4) ls command
LS means List files. it shows teh files and directory within a system.
'ls -R' shows all files in the subdirectories
'ls -a' shows all hidden files (dot files) in addition to the visible ones
'ls -1h' shows files and their sizes in readble format

see output below

![](Images/4-LS%20commands.PNG)

### 5) cat Command
'cat' means Concatenante. It is used for reading, listing , combining and writing file contents to standard output.

'cat filename1.txt filename2.txt > filename4.txt'  was use to merge text files with name filename1 and filename2 to filename4 as shown below

![](Images/5-cat%20commands.PNG)

### 6) CP Command
CP means copy. used for copying files or directory and their contents
the following commands were used to practice

i) 'cp sqlite_commands.sh /home/ubuntu/unixcommands' to copy sqlite_commands.sh file from home ubuntu directory to unixcommands2 directory

ii) cp filename1.txt filename2.txt filename3.txt /home/ubuntu/documents' was used to copy the three files in txt format  from ubuntu directory to documents directory

iii) cp filename1.txt filename2.txt  was ued to copy content in filename1.txt to filename2.txt

iv) cp -R /home/username/documents /home/username/document_backup  was used to the entire directory in documents fo document_backup

Output Details shown below

![](Images/6-CP%20commands.PNG)


### 7) mv Command
mv means move.  Primarily used for moving and renaming files and directories. Two commands were used in the output below
i) mv sqlite_commands1.sh /home/ubuntu/CommandsLinux to move the .sh file from it's current ubuntu directory to commandsLinux directory
ii) mv sqlite_commands.sh sql_commands.sh was used to rename sqlite_commands.sh to sql_commands.sh

![](Images/7-mv%20command.PNG)


### 8) mkdir commnad
mkdir means make directory. For creating a new directory.
'mkdir Music' command was used to create a new directory called Music
'mkdir Music/Songs' command was used to create a new directory called Songs inside Music directory

![](Images/8-mkdir%20command.PNG)


### 9) rmdir Command
rmdir means remove directory. it's used for permanently deleting an empty directory.
'rmdir -p Music/Songs' command below was used to remove both music directory and it's empty subdirectory named Song

![](Images/9-rmdir%20command.PNG)


### 10) rm Command
rm means remove file within a directory. it's used for deleting files with a directory.

rm filename  command was used to remove the file namekd  filename inside ubuntu directory
rm filename1 filename2 filename3  command was used to remove multiple files filename1 filename2 and filename3 from Ubuntu directory

See output below

![](Images/10-rm%20command.PNG)


### 11) touch Command
touch command is used for creating an empty file as shown below

 'touch sqlite_commands.sh' used for creating a new file named sqlite_commands.sh

 ![](Images/11-%20touch%20command.PNG)


 ### 12) locate command
'locate -i filename3.txt'  command is used for searching for files that contain words filename3.txt
"-r' arguements will turn off case sensitivity

![](Images/12%20-%20locate.PNG)
 
 
 ### 13) find command
 find command is used for looking for files within a directory and it's subfolders.
 
'find /home -name sql_commands.sh'  commadn was used to find a file called sql_commands.sh

![](Images/13-%20find.PNG)

### 14) grep command
it's used for finding a word by searching through all the text in a specific file. I copied some words into the filename3.txt using nano editor.

'grep LTE filename3.txt' was used to look for all the word "LTE'in the text file called filename3.txt.

![](Images/14%20grep.PNG)


### 15) df command 
used to report the system disk space usage

df -h give teh output below

![](Images/15%20df.PNG)

### 16) du command
To check how much space a file or directory takes up.
The directory of the file must be specified

du /home/ubuntu/commandsLinux give the output below

![](Images/16%20du.PNG)


### 17) head command
Allows users to view the first few lines of a text. 

'head filename3.txt' shows the first five lines of the content of filename3.txt

![](Images/17%20head.PNG)


### 18) tail command
Allows users to view maximum of the last ten lines of a text, incase another upade has been added

 tail filename3.txt  shows the first six lines of the content of filename3.txt
tail -n filename3.txt was used to specify the number of lines to view
 
![](Images/18%20tail.PNG)


 ### 19) diff command
 diff represents difference commands which is used for comparing the two contents of a file. It dispalys the parts that do not match.

 diff filename2.txt filename3.txt command was used to compare teh content of the two files named filename2.txt and filename3.txt.
 the difference was dispalyed in the output below

 ![](Images/19%20diff.PNG)


 ### 20) tar command 
 tar command is use for chiving files similar to ZIP function.
 basic syntax :  tar [options] [archive_file] [file or directory to be archived]

 tar -cvf newarchive.tar /home/ubuntu command give the output below

 ![](Images/20%20tar.PNG)


 ## FILE PERMISIION AND OWNERSHIP

 ### 21) chmod command
 chmod command modified a file or directory's read , write and execution permissions. to allow all group members to be able to read, write and execute a file, change the perssion to -rwxrwxrwx using 777 e.g chmod 777 filename3.txt
 'ls -ltr' commnad was first used to check the permisison on the files before making changes. See output below

 ![](Images/21%20chmod.PNG)


 ### 22) chown command
 chown command is used to change the ownership of a file , directory or symbolic link.
 'chown linuxuser2 filename.txt' command will assign ownership of filename.txt to linuxuser2. before using this commnad "ls -l" is used to check the current owner as shwon below (note ubuntu is the owner of the file and couldnt change it)

 ![](Images/22%20chown.PNG)

 ### 23) jobs command
 It's used for displaying all running processes- along with their statuses
 jobs [options] jobID


### 24) kill command
used for terminating an unresponsive program manually. To kill a program , the process identification number (PID) must be known by running "ps ux". 
The default signal option used with KILL is SIGKILL which forces the program to stop.

kill SIGKILL 22056 - (I only showed the command but didnt kill any program since it is not mine)

![](Images/24%20kill.PNG)


### 25) ping command
used for checking ifa server is reachable or troubleshoot various connectivity issues
syntax : ping [option] [hostname_or_IP_address]

ping google.com was used in the output below
CTRL+C was used to stop the ping command

![](Images/25%20Ping.PNG)


### 26) wget command
it is used for downloading files from internet (HTTP, HTTPS and FTP);it works in the background.

![](Images/26%20wget.PNG)


### 27) uname command
It's used for printing detail information about the linux system and hardware

uname -a (for system information) ,   uname -s (prints kernel)   uname -n (prints the system node hostname) as shown below

![](Images/27%20uname.PNG)


### 28) top command 
For displaying all running processes and real time view of the current system.
CTRL+C was used to stop the command

![](Images/28%20top.PNG)

### 29) history command
list all the previously executed commands, up to 500

![](Images/29%20history.PNG)

### 30) man command
It provides user manual for any command you can run on the linux terminal

' man ls'

![](Images/30%20b.PNG)


### 31) echo command 
When echo command is used with a line of text or string , it displays the line of text as output. It supports other options when used with flags

![](Images/31%20Echo.PNG)


### 32) zip , unzip commands
for compressing file into ZIP file (and decompressing file)

![](Images/32%20zip%20unzip.PNG)


### 33) hostname command
For determining the system's hostname as shwon below
hostname [option]  it works with -1 , -a , -all as shown below


![](Images/33%20hostname.PNG)


### 34) useradd , userdel commands
Useradd is used for creating a new account; passwd used for creating a new password; userdel is used for deleting a user account
root or sudo privileges is required to run the command

useradd [option] username.
I had to sudo to the useradd command to have required permisison as shown below

![](Images/34%20useradd.PNG)


### 35) apt-get command
The command is used for Advanced Package Tool(APT) libraries in Linux. It helps in retrieving information from reliable sources to manage, update , remove , and install  software and it's dependecies.

'apt-get'

![](Images/35%20apt-get.PNG)


### 36) nano , vi , jed commands
The commands allows users to edit and manage files via text editor

'nano filename2.txt'  to exit and save press CTRL + X and press enter

'vi filename2.txt'  to save in vi type :w and hit Enter , to exit type :x and hit Enter key.

![](Images/36%20nano.PNG)

 
### 37) alias , unalias command
alias allows you to create a shortcut with the same functionality as the command.

alias K='KILL'

unlias K

![](Images/37%20alais.PNG)


### 38) su command
su means switch user, allows one to runa a program as a new user. It helps to access the system through SSH when the rootuser is unavailable. it will as k for the existing user's password for you to proceed

su [options] [username [argument]]

'su ubuntu' was used for the practice

![](Images/38%20su.PNG)


### 39) htop command 
It is used for monitoring shystem resources and server processes in real time

'htop'

![](Images/39%20htop.PNG)


### 40) ps commands
It shows snap shot of all running processes in the system
It can be used with flags like -T(all process linked to current shell) , -A (all running process) , -u username (process linked to a specific username)

The below command is displayed in the output below

'ps -T'

'ps -A'


'ps -u username'

![](Images/40%20ps.PNG)

















