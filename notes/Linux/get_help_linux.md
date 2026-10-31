# Get Help in Linux

## man
Displays the full manual page.
```bash
man grep
man chmod
man tcpdump
```
Useful keys in `man`:
- `/pattern`: search
- `n`: next result
- `q`: quit

## whatis
Displays a brief one-line description.
```bash
whatis grep
whatis chmod
```
## apropos
Searches manual-page names and descriptions.

```bash
apropos password
apropos permission
apropos network
```
## help
Displays help for shell built-in commands.

```bash
help cd
help echo
```
## Command-Specific Help

```bash
grep --help
find --help
python3 --help
```

## Recommended Workflow
1. Try `command --help` for a quick option list.
2. Use `man command` for details.
3. Use `whatis` for a short definition.
4. Use `apropos keyword` when the command name is unknown.
5. Test unfamiliar commands in a safe lab before using them on important files. 


Command | Purpose | Example
--------|---------|--------
man | Displays information on other commands and how they work; Open full manual page. The output is called a “man page,” which is short for "manual page" | man chown Displays detailed information about chown and how it works
whatis | Displays a description of a command on a single line | whatis nano Displays the description of nano on a single line
apropos | Searches the manual page descriptions for a specified string | apropos password Returns the manual pages of commands that contain the keyword password; apropos -a graph editor Returns the manual pages of commands that contain both the keywords graph and editor; the -a option specifies to only return commands that contain all specified strings
help | display help for shell built-ins | help cd




