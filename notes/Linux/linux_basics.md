# Linux Shells

## What is a Shell?

A Shell is a command-line interpreter that allows users to interact with the operating system.

## Common shells

Shell | Description |
------|-------------|
Bash | Most common Linux shell|
Sh | Original Bourne Shell|
Zsh | Default shell on modern macOS |
PowerShell | windows command shell |

## Linux Components
- Kernel: manages hardware, processes, memory, and system resources.
- Shell: command-line interface between user and operating system.
- File system: organizes files and directories.
- Distribution: packaged Linux operating system such as Ubuntu, Debian, or Kali Linux.


## File-System Structure

| Directory | Purpose |
|---|---|
| `/` | Root of the file system |
| `/home` | User home directories |
| `/etc` | System configuration |
| `/var/log` | Log files |
| `/bin` and `/usr/bin` | Commands and programs |
| `/tmp` | Temporary files |


## Absolute and Relative Paths

- Absolute path starts at `/`.
- Relative path starts from the current directory.

```bash
pwd
cd /var/log
cd ../
cd ./reports
```
## Security Relevance
Linux is commonly used for servers, cloud workloads, security tools, log analysis, scripting, and incident response. 

## Key Difference

Terminal = Application window

Shell = command interpreter


# Shell Basics

Command | Purpose  | Example
--------|----------|--------|
Echo | Display text | echo "Hello Linux"
Expr | Perform arithmetic | expr 10 + 5 
clear | Clear terminal screen | clear
