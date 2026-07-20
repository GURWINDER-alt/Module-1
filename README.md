#  Module-1
## Topics Covered
# Module 1: Fundamentals of Unix/Linux & BASH Essentials

## 1. Introduction to Linux
# What is Linux?
Linux is a free and open-source operating system based on the Unix operating system. It was created by Linus Torvalds in 1991. Linux acts as a bridge between the computer hardware and the user, allowing users to run programs, manage files, and control hardware resources.
Unlike Windows and macOS, Linux is open source, meaning anyone can view, modify, and distribute its source code.
# Features
Free and open source
Multi-user (many users can use it simultaneously)
Multitasking (runs multiple programs at the same time)
Secure and stable
Portable (works on different hardware)
Fast performance
Strong networking support
# Advantages
No license cost  
Highly secure against viruses  
Stable for long-running servers  
Customizable  
Used in cloud computing, supercomputers, Android, IoT, and web servers  
# Popular Linux Distributions  
Ubuntu  
Debian  
Fedora  
Linux Mint  
Kali Linux  
Arch Linux  
Red Hat Enterprise Linux (RHEL)  
# 2. Linux Installation
Linux can be installed in two ways.  
A. Virtual Machine Installation  
A Virtual Machine (VM) allows you to run Linux inside Windows without changing your computer.  
# Software Required
VirtualBox  
VMware  
Ubuntu ISO file  
# Steps
Download Ubuntu ISO.  
Install VirtualBox.  
Create a new virtual machine.  
Allocate RAM and storage.  
Attach the Ubuntu ISO.    
Start the VM.  
Complete Ubuntu installation.  
# Advantages
Safe  
Easy to remove  
Good for learning  
No risk to Windows  
B. Bare Metal Installation  
Linux is installed directly on the hard disk.  
# Types:
Full Disk Installation  
Dual Boot (Windows + Linux)  
# Advantages
Better performance  
Full hardware access  
Partitioning  
A partition divides the hard disk into separate sections.  
MBR (Master Boot Record)  
Maximum disk size: 2 TB  
Maximum 4 primary partitions  
# Older partitioning method  
GPT (GUID Partition Table)
Supports disks larger than 2 TB
Up to 128 partitions  
More secure  
Used with UEFI systems  
# Important Linux Partitions
/  
The root directory. Every file and folder starts here.  
/home  
Stores personal files of users.  
Example  
/home/sara/Documents  
/boot  
Contains files needed to start Linux.  
swap  
Used as virtual memory when RAM becomes full.  
# 3. Introduction to BASH & Linux Command Line  
# What is Shell?  
A Shell is a program that accepts commands from the user and sends them to the operating system.  
Examples  
Bash  
Zsh  
Fish  
Ksh  
# What is BASH?
BASH stands for  
Bourne Again SHell  
It is the default command-line interpreter in most Linux distributions.  
# Functions
Executes commands  
Runs shell scripts  
Automates repetitive tasks  
# 4. Linux File System Structure  
Linux uses a hierarchical tree structure.  
/  
├── bin  
├── boot  
├── dev  
├── etc  
├── home  
├── var  
├── usr  
├── tmp  
 Important Directories  
/  
Root directory  
/home  
Stores user data.  
/etc  
Contains configuration files.  
/var  
Stores log files, mail, cache, etc.  
/usr  
Contains installed software and libraries.  
/bin  
Stores essential commands like  
ls  
cp  
mv  
/tmp  
Temporary files.  
# 5. File and Directory Permissions  
Linux protects files using permissions.  
Permission Types  
Read (r)  

Write (w)  

Execute (x)  
There are three users  
Owner  
Group  
Others  
Example  
-rwxr-xr--  
Meaning  
Owner → rwx  
Group → r-x  
Others → r--  
chmod Command  
Changes permissions.  
Example  
chmod 755 file.txt  
chown Command
Changes file ownership.
Example
sudo chown user file.txt
# 6. Basic File Operations
pwd  
Shows current directory.  
pwd  
ls  
Lists files.  
ls  
cd  
Changes directory.  
cd Documents  
mkdir  
Creates directory.  
mkdir Linux   
touch  
Creates file.   
touch notes.txt  
cp  
Copies files.  
cp file1 file2  
mv  
Moves or renames files.  
mv old.txt new.txt  
rm  
Deletes files.  
rm file.txt  
7. Redirection and Pipes  
>  
Redirects output to a file.  
ls > files.txt  
>>  
Appends output.  
echo Hello >> notes.txt  
<  
Reads input from a file.  
sort < numbers.txt   
Pipe (|)  
Passes output of one command to another.  
ls | grep txt  
8. Wildcards  
Wildcards match filenames.  
*  
Matches many characters.  
*.txt  
?   
Matches one character.  
file?.txt  
[]  
Matches specific characters.  
file[123].txt  
9. Quoting and Escaping Characters  
Single Quotes  
Everything inside is treated literally.  
echo 'Hello $USER'  
Output  
Hello $USER  
Double Quotes  
Variables are expanded.  
echo "Hello $USER"  
Output  
Hello Sara  
Escape Character ()  
Treats the next character literally.  
echo \$100  
Output  
$100  
10. Bash Scripting  
A Bash script is a file containing Linux commands executed one after another.  
Example  
#!/bin/bash  

echo "Hello World"  
Save as  
hello.sh  
Run  
bash hello.sh  
Variables  
name="Sara"  

echo $name  
Input  
read name  
 
echo $name  
Conditional Statement  
if [ $age -ge 18 ]  
then  
echo "Adult"  
else  
echo "Minor"  
fi  
# 11. Using man and help   
man  
Displays the manual page of a command.  
man ls  
help  
Shows help for Bash built-in commands.  
help cd  
12. Text Processing Tools  
grep  
Searches for text.  
grep "Linux" notes.txt  
awk  
Processes text column by column.  
awk '{print $1}' file.txt  
sed  
Edits text automatically.  
sed 's/Linux/Ubuntu/g' file.txt  
13. File Compression  
tar  
Creates an archive.  
tar -cvf backup.tar folder/  
gzip  
Compresses a file.  
gzip file.txt  
zip  
Creates a ZIP archive.  
zip files.zip file1 file2  
unzip  
Extracts ZIP files.  
unzip files.zip  
# Real-Life Applications of Module 1
Software Development: Developers use Linux and Bash to write, test, and deploy applications.  

Cloud Computing: Most cloud servers (AWS, Azure, Google Cloud) run Linux.  

Cybersecurity: Ethical hackers and penetration testers use Linux distributions like Kali Linux.  

System Administration: Administrators manage users, permissions, backups, and servers using Linux commands.  

Automation: Bash scripts automate repetitive tasks such as backups, file management, and software installation.  

Data Processing: Tools like grep, awk, and sed quickly search and process large log files and datasets.  

DevOps: Linux and Bash are essential for CI/CD pipelines, Docker, Kubernetes, and server management.  

