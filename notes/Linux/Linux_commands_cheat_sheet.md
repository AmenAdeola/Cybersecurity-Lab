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


# Searching & Filtering

Commands | Purpose | Example Result|
--------|---------|----------------|
grep | search text in files |grep error logs.txt
grep -c | count matching lines | grep -c warning logs.txt
grep -i | ignore case |grep -i error logs.txt
grep -ic | count matches ignoring case| grep =ic warning logs.txt
` |`|Pile output to another command|
wc -l| count lines |ls |grep access | wc -l
find | search files and directories |find /home/analyst/projects
find -name | search file names (case-sensitive)| find . -name "*log*"
find -iname |search file names (case-isensitive)|find . -iname "*log*"
find -mtime| search by modification days|find . -mtime -3
find -mmin | search by modification minutes |find . -mmin -30

# File & directory management

Commands | Purpose | Example Result|
--------|---------|----------------|
mkdir | Create a directory |mkdir logs
rmdir | Remove an empty directory | rmdir temp
mv | move or rename file /directory |mv Q3patches.txt reports/
rm | delete a file |rm tempnotes.txt|
touch| create an empty file |touch tasks.txt
nano | edit a file | nano tasks.txt


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








