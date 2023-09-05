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


 ### 19) 

















