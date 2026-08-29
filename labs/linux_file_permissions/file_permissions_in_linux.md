# Project Description

In this activity, I reviewed file and directory permissions in a linux environment and verified that access controls aligned with organizational  security policies. Using Linux commands, I inspected permissions, identified excessive access rigths, and modified permission to support the principle of least privilege. This activity strenghtened my ability to manage access control and  secure sensitive files and directories.

# Check file and directory details

Command: ls -la

Description:
I used  the ls -la command to display all files directories, including hidden files, and review their permissions, ownership, and associated groups. 

This command displayed the file permission strings for files in the projects directory, including project_k.txt, project_m.txt, project_r.txt, project_t.txt,.project_x.txt, and the drafts directory.

Example from file:

project_k.txt 
-rw-rw-rw-

#Describe the permissions string

Example: -rw-rw-rw-
Description:

The first character (-) indicates that the item ia a regular file

characters 2-4 (rw-) represent the user permissions, allowing the owner to read and write.

characters 5-7 (rw-) represent the group permissions, allowing members of the group to read and write.

Characters 8-10 (rw-) represent permissions for others, allowing all other users to read and write.

The permission string indicates that the file can be read modified by owner, the group and all other users.

# Change file permissions

project_k.txt

user = read, write
group = read, write
other = read, write

organization don't allow others = write

command: chmod o-w project_k.txt

I used chmod o-w project_k.txt to remove write permissions for other users while preserving existing user and group permissions.

This change reduced unnecessary access and aligned permissions with the principle of least privilege

# Change file permissions on a hidden file

folder: .project_x.txt
current permissions:
user = read, write
group = write
other = none

scenario says: They do not want anyone to have write access to this project, but the user and group should have read access.
command: chmod u-w, g-w, g+r .project_x.txt
Description: I modified the permissions of the hidden file. .project_x.txt so that the owner retained read and write permissions while the group received read-only access. Others users were given no permissions.

# Change directory permissions
current situation: 
Drafts
user = read, write, execute
Group = execute
Other = none
Scenario: Only researcher2 should have access.
command: chmod g-x drafts
Description: I used chmod g-x drafts to remove execute permissions for the group. This restricted access to the drafts directory so that only the owner could access its contents

# Summary

In this activity, I reviewed Linux file and directory permissions and identified permissions that did not comply with organizational security requirements. Using ls -la and chmod, I inspected permissions and modified access rights to enforce the principle of least privilege.

I removed unnecessary write and execute permissions, secured hidden files, and restricted access to sensitive directories. These actions reduced the risk of unauthorized access and improved the overall security of the file system
