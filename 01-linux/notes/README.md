# Linux Fundamentals

## Key Concepts

- Linux is a Unix-like operating system
- Everything in Linux is treated as a file
- The system is case-sensitive
- The root user has full administrative privileges

## Commands

`whoami` - display current user  
`hostname` - show system hostname  
`uname -a` - display system information  

## Examples

whoami
uname -a

## What I Learned

- Understanding the system environment is the first step in working with Linux
- User context matters for permissions and operations


# File and Directory Management

## Key Concepts

- The filesystem is hierarchical
- Paths can be absolute or relative
- Directories store files and other directories

## Commands

`ls` - list directory contents  
`cd` - change directory  
`pwd` - print current directory  
`mkdir` - create directory  
`rm` - remove files or directories  
`cp` - copy files  
`mv` - move or rename files  

## Examples

ls -la
cd /var/log
mkdir project
rm file.txt

## What I Learned

- Efficient navigation is essential for productivity
- File operations form the basis of most Linux tasks


# File Permissions

## Key Concepts

- Permissions control access to files and directories
- Three permission groups: user, group, others
- Permission types: read, write, execute

## Commands

`ls -l` - view permissions  
`chmod` - change permissions  
`chown` - change file ownership  

## Examples

chmod 755 script.sh
chown user:group file.txt

## What I Learned

- Permissions are critical for system security
- Misconfigured permissions can expose systems to risk


# Processes and System Monitoring

## Key Concepts

- A process is a running instance of a program
- Each process has a unique PID
- Monitoring helps manage system performance

## Commands

`ps aux` - list processes  
`top` - real-time process monitoring  
`htop` - interactive process viewer  
`kill` - terminate a process  

## Examples

ps aux | grep nginx
kill 1234

## What I Learned

- Managing processes helps maintain system stability
- Identifying resource-heavy processes is important


# Networking Basics

## Key Concepts

- IP addresses identify devices on a network
- Ports enable communication between services
- Networking tools help diagnose connectivity

## Commands

`ip a` - show IP addresses  
`ping` - test connectivity  
`ss -tuln` - list open ports  

## Examples

ping google.com
ss -tuln

## What I Learned

- Networking knowledge is essential for troubleshooting
- Open ports can indicate running services


# Package Management

## Key Concepts

- Software is installed via package managers
- Repositories provide verified software
- Keeping systems updated is important for security

## Commands

`apt update` - update package list  
`apt upgrade` - upgrade installed packages  
`apt install` - install new package  
`apt remove` - remove package  

## Examples

sudo apt update
sudo apt install nginx

## What I Learned

- Package managers simplify software management
- Regular updates reduce security risks


# Text Processing and Redirection

## Key Concepts

- Output can be redirected to files
- Commands can be chained using pipes
- Text processing is essential for log analysis

## Commands

`>` - overwrite output  
`>>` - append output  
`|` - pipe output  
`cat` - display file contents  
`less` - view file interactively  
`grep` - search for patterns  

## Examples

cat file.txt | grep error
echo "hello" > file.txt

## What I Learned

- Combining commands increases efficiency
- Text processing tools are powerful for automation


# Logs and System Files

## Key Concepts

- Logs store system and application activity
- Useful for debugging and monitoring
- Important for security investigations

## Common Locations

/var/log/syslog  
/var/log/auth.log  
/var/log/nginx/

## Commands

`tail` - view end of file  
`tail -f` - monitor logs in real time  

## Examples

tail -f /var/log/syslog

## What I Learned

- Logs provide insight into system behavior
- Monitoring logs helps detect issues early