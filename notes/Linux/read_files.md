# Read Files 

## cat  
```bash 
cat auth.log
```
Displays the full file. Best for short files.  

## head  
```bash 
head server_logs.txt
head -n 5 server_logs.txt
```
Displays the beginning of a file.  

## tail  
```bash 
tail auth.log
tail -n 20 auth.log
tail -f application.log
```
Displays the end of a file. `-f` follows new entries.  

## less  
```bash 
less server_logs.txt
```
Useful for large files.  

- `/pattern`: search
- `n`: next match
- `q`: quit

## Security Workflow  
```bash
head auth.log 
tail -n 50 auth.log
grep FAILED auth.log
less auth.log
```
Preserve original log files and avoid commands that overwrite evidence. 

commands | purpose | Example|
---------|---------|--------|
cat | Displays the content of a file |cat updates.txt: Displays the content of the updates.txt file
head |Displays just the beginning of a file, by default 10 lines | head updates.txt: Displays only the first 10 lines of the updates.txt file; head -n 5 updates.txt: Displays only the first five lines of the updates.txt file; the -n option allows users to specify the number of lines to return
less | Returns the content of a file one page at a time | less updates.txt: Returns the content of updates.txt one page at a time; the less command changes the terminal window to a display that allows users to easily move forward and backward through content
tail | Displays just the end of a file, by default 10 lines | tail updates.txt: Displays only the last 10 lines of the updates.txt file; tail -n 5 updates.txt: returns only the last five lines of the updates.txt file; the -n option allows users to specify the number of lines to return




