# Filter content commands

Commands | Purpose | Example Result|
--------|---------|----------------|
find | Searches for directories and files that meet specified criteria| find /home/analyst/projects: Searches for all files starting at the projects directory; find /home/analyst/projects -name "*log*": Searches for all files in the projects directory that contain the word log in the file name; the -name option searches for a specified string and is case-sensitive; the * wildcard represents zero or more unknown characters; find /home/analyst/projects -iname "*log*": Searches for all files in the projects directory that contain the word log in the file name; the -iname option searches for a specified string and is not case-sensitive; the * wildcard represents zero or more unknown characters; find /home/analyst/projects -mtime -3: Searches for all files in the projects directory that have been modified within the past three days; the -mtime option bases its search for files or directories that were modified on days; find /home/analyst/projects -mmin -15: Searches for all files in the projects directory that have been modified within the past 15 minutes; the -mmin option bases its search for files or directories that were modified on minutes
grep | Searches a specified file and returns all lines in the file containing a specified string| grep OS updates.txt: Searches the updates.txt file and returns all lines containing the string OS; grep -c counts matching lines: grep -c warning logs.txt; grep -i ignores case: grep -i error logs.txt; grep -ic counts matches ignoring case: grep =ic warning logs.txt; 
I=piping | Pile output to another command, Sends the standard output of one command as standard input to another command for further processing; accessed using the pipe character (I) | ls /home/analyst/reports I grep users redirects the standard output of ls /home/analyst/reports to be standard input for the grep users command, meaning that grep users identifies files and subdirectories in the /home/analyst/reports directory that contain the string users within their file name
wc -l| count lines | grep access logs.txt I wc -l


 ## grep
 ```bash
grep ERROR server_logs.txt
grep -i error server_logs.txt
grep -n WARNING server_logs.txt
grep -c FAILED auth.log
grep -v INFO application.log
```
| Option | Purpose |
|---|---|
| `-i` | Ignore case |
| `-n` | Show line numbers |
| `-c` | Count matching lines |
| `-v` | Show non-matching lines |
| `-r` | Search recursively |

## Pipes
A pipe sends the output of one command to another.
```bash
ls -la | grep access
grep WARNING logs.txt | wc -l
cat auth.log | grep FAILED | sort
```
## find
```bash
find . -name "*.log"
find . -iname "*report*"
find . -type f
find . -type d
find . -mtime -3
find . -size +10M
```
## Security Use Cases
- Locate logs and configuration files.
- Count failed login events.
- Find files modified recently.
- Search for usernames, IP addresses, hashes, or error messages.
- Reduce large command output to relevant evidence. 
