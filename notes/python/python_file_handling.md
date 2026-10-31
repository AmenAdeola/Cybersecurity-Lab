# Python File Handling  

## Open Files Safely  
```python 
with open("allow_list.txt", "r") as file:
     data = file.read()
```

The `with` statement closes the file automatically.

## Modes

| Mode | Purpose |
|---|---|
| `r` | Read |
| `w` | Write or overwrite |
| `a` | Append |
| `r+` | Read and write |

## Parse Text
```python
ip_addresses = data.split()
```
## Update a List
```python
for element in remove_list:
     if element in ip_addresses:
         ip_addresses.remove(element)
```
## Convert Back to Text
```python
updated_text = " ".join(ip_addresses)
```
 
 ## Write the File
 ```python
 with open("allow_list.txt", "w") as file:
     file.write(updated_text)
```
 ## Workflow
```text
Open → Read → Parse → Modify → Join → Write → Verify
```

## Security Considerations
- Preserve the original when required.
- Validate input and output paths.
- Avoid overwriting evidence.
- Handle missing files or invalid data.
- Do not store secrets in source code. 
