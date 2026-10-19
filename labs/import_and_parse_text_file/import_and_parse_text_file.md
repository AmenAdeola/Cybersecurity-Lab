# Import and Parse a Text File 

## Objective

Read, parse, append, create, and write security-related text files.

## Core Code and Explanation

```python
with open(import_file, "r") as file:
     text = file.read()
  items = text.split()
  with open(import_file, "a") as file:
     file.write(missing_entry)
  with open("allow_list.txt", "w") as file:
     file.write(ip_addresses)
```

Use `with` so the file closes automatically. 
Read mode is `r`, write mode is `w`, and append mode is `a`.  

## Key Takeaways

The lab combines foundational Python syntax with a security scenario. Keep the code, observed output, answers to reflection questions, and a short security relevance section in the GitHub file.

## Skills Demonstrated  

- Python
- Cybersecurity automation
- Problem solving
- Code documentation 

