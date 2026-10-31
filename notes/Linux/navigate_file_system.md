# Navigate the File System

## Core Commands  

```bash 
whoami
pwd
ls
ls -l
ls -la
cd /var/log
cd ..
cd ~
```

## Symbols  
| Symbol | Meaning |
|---|---| 
| `/` | Root directory | 
| `~` | Current user home directory | 
| `.` | Current directory | 
| `..` | Parent directory |  

## Examples  
```bash
cd /home/analyst/reports
pwd
ls -la
cd ../logs
```

## Analyst Workflow  

1. Confirm identity with `whoami`.
2. Confirm location with `pwd`.
3. List files with `ls -la`.
4. Move deliberately using `cd`.
5. Reconfirm location before deleting, moving, or changing permissions. 


Command | Purpose | Example
--------|---------|-------|
cd | Navigates between directories| cd reports : Navigates from the current working directory to its subdirectory reports; cd /home/analyst/reports: Navigates to the reports directory; the full path is required when reports is not a subdirectory of the current working director; cd .. : Navigates to the directory that is one level above the current working directory
ls| Displays the names of the files and directories | ls:	Displays the names of the files and directories in the current working directory; ls /home/analyst/reports: Displays the names of the files and directories in the reports directory; providing an argument that specifies the path to a directory is necessary to display the contents of a directory other than the user's current working directory; ls -a: Displays hidden files when displaying the names of files and directories inside the current working directory; ls -l: Displays permissions to files and directories in the current working directory; also displays other additional information, including owner name, group, file size, and the time of the last modification; ls -la: Displays permissions to files and directories in the current working directory, including hidden files; also displays other additional information, including owner name, group, file size, and the time of last modification
pwd | Prints the working directory to the screen| pwd : Prints the working directory to the screen, such as /home/analyst
whoami | Returns the username of the current user| whoami; Returns the username of the current user, such as analyst or fgarcia
