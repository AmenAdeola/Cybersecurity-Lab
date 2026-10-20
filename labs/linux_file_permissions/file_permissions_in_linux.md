# Linux File Permissions

# Project Description

In this activity, I reviewed file and directory permissions in a linux environment and verified that access controls aligned with organizational  security policies. Using Linux commands, I inspected permissions, identified excessive access rigths, and modified permission to support the principle of least privilege. This activity strenghtened my ability to manage access control and  secure sensitive files and directories.

## Objective

Inspect hidden files, interpret permission strings, and change permissions according to requirements.

## Inspect Permissions  ```bash pwd ls -la ```  `ls -la` shows hidden files, file types, permissions, owner, group, size, and modification information.

## Interpret the Permission String

Example: `-rw-r-----`
- First character: file type
- Characters 2–4: user permissions
- Characters 5–7: group permissions
- Characters 8–10: other permissions
- `r`: read, `w`: write, `x`: execute, `-`: permission absent

## Modify Permissions
```bash
chmod u=rw, g=r, o= project_k.txt
chmod 640 project_k.txt
chmod o-r hidden_file.txt
```
Symbolic mode is useful when the required changes are expressed by user, group, and other. Numeric mode is useful for concise repeatable settings.

## Directory Permissions

For a directory, read lists names, write permits creating or deleting entries, and execute permits entering/traversing the directory.

## Security Relevance

Least privilege reduces unauthorized disclosure, modification, and execution. Permission changes should be validated with `ls -la` after each update.

## Skills Demonstrated

- Linux
- File permissions
- Least privilege
- User and group permissions
- Command-line administration 

# Summary

In this activity, I reviewed Linux file and directory permissions and identified permissions that did not comply with organizational security requirements. Using ls -la and chmod, I inspected permissions and modified access rights to enforce the principle of least privilege.

I removed unnecessary write and execute permissions, secured hidden files, and restricted access to sensitive directories. These actions reduced the risk of unauthorized access and improved the overall security of the file system

