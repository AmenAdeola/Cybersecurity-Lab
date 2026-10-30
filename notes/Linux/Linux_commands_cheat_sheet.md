# Linux Commands Cheat Sheet

# Package Management (APT, Advanced Package Tool)

Command | Purpose | Example Result |
--------|---------|----------------|
apt     | Displays package manager help and available commands | APT usage information|
apt --version | displays the installed APT version | apt 2.2.4 |
sudo |run command with administrator privileges |
apt install | Install a package/softaware|
apt --installed | displya installed packages|
apt remove | Remove a package software|
apt search | Search for available packages|
apt update | Update package lists |
apt upgrade| Upgrade installed packages|
suricata | Run the suricata application
sudo apt install tcpdump | Install tcpdump|
tcpdump | Capture and analyze network traffic|
sudo apt remove suricata | Uniistall Suricata |
tcpdumo | Network traffic capture tool, package capture & Traffic analysis|
apt list --intalled | Display installed packages
apt search <packages> | search available packages|
sudo apt install <packages> | install a package|
sudo apt remove <packages>| remove a package|
suricata|IDS/IPS detect and prevent network threats


## Navigation
```bash
whoami
pwd
ls
ls -la
cd
/path
cd ..
cd ~
```
## Read Files
```bash
cat file.txt
head file.txt
head -n 5 file.txt
tail file.txt
less file.txt
```
## Manage Files and Directories

```bash
touch report.txt
mkdir logs
rmdir empty_folder
mv source destination
rm file.txt
nano report.txt
```

## Search and Filter
```bash
grep ERROR server_logs.txt
grep -c WARNING server_logs.txt
grep -i error logs.txt
ls | grep access
find . -name "*log*"
find . -iname "*log*"
find . -mtime -3
```
## Users and Permissions
```bash
ls -l
chmod u=rw,g=r,o= report.txt
chmod 640 report.txt
sudo chown analyst1 report.txt
sudo chgrp security report.txt
sudo useradd analyst1
sudo usermod -a -G security analyst1
sudo userdel analyst1
```
## Help
```bash
man grep
whatis chmod
apropos password
help cd
```
## Integrity and Network
```bash
sha256sum file.txt
cmp file1hash file2hash
sudo tcpdump -D
sudo tcpdump -i eth0 -v -c 5
sudo tcpdump -i eth0 -nn -w capture.pcap
sudo tcpdump -nn -r capture.pcap -X
``` 







# Linux commands cheat sheet

Commands | Purpose | Example Result|
--------|---------|----------------|
whoami  | Displays the current logged-in user| analyst|
pwd     | Displays the current working directory | /home/analyst |
ls | List files and directories | ls|
ls <directory> | list contents of a specific directory |ls reports|
cd <directory> |change directory |cd reports|
cd .. |move to parent directory | cd.. |
cd ~ | Return to home directory |cd ~|
cat | display file contents| cat tasks.txt|
head | Display first 10 lines of file | head server_logs.txt
head -n 5 | display first N lines | head -n 5 server_logs.txt
tail | display last 10 lines of file | tail server_logs.txt
less | view file page by page | less server_logs.txt
echo |dislay text output |echo "hello"
expr | Perform calculations| expr 32 - 8
clear | clear terminal screen |clear 

# Commands Line shortcuts

Shortcut | Purpose | 
--------|---------|
Ctrl + C| Cancel current command
Ctrl + U |Delete everything before cursor
Ctrl + K | Delete everything after cursor
Ctrl + W | Delete previous word
Backspace| Delete previous character


# Nano Editor Shortcuts

Shortcut | Purpose | 
--------|---------|
Ctrl + X | Exit Nano
Y | Save changes
Enter | Confirm file name
Ctrl + O | write file (save)


# Linux Permissions cheat sheet

Permission Types

Permission | Symbol | Files | directories
-----------|--------|-------|------------|
Read | r | Read file contents | View directory contents
Write| w | Modify file contents | create/delete files
Execute| x | Execute program | Enter directory

# Ownership Types

Owner Type | Symbol | Description
-----------|--------|-------------
User | u | File owner
Group | g | Owner's group
Other | o | All other users

# Permissions String Structure
Example: drwxrwxrwx

Position | Meaning 
---------|----------|
1 | File type (d=directory, -= regular file
2-4 | Users permissions |
5-7 | Group permissions
8-10 | Other permissions

example: -rw-r-----
interpretation: 
File
User: Read + Write
Group: Read only
Other: No access

# Permission Inspection commands

Commands | Purpose | Example|
---------|---------|--------|
ls -l | display permissions, owner, group, size, date | ls -l
ls -a | display hidden files | ls -a
ls -ls| dispaly hidden files with permission | ls -la
stat | afficher les metadonnees detailles d<un fichier | stat rapport.txt








