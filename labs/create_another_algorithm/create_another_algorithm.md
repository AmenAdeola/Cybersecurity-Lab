# Create Another Algorithm  

## Objective

Remove deauthorized IP addresses from an allow-list file.  

## Core Code and Explanation  
  ```python 
def update_file(import_file, remove_list):     
  with open(import_file, "r") as file:         
    ip_addresses = file.read()      
  ip_addresses = ip_addresses.split()      
for element in remove_list:         
  if element in ip_addresses:             
    ip_addresses.remove(element)      
ip_addresses = "\n".join(ip_addresses)      
with open(import_file, "w") as file:         
  file.write(ip_addresses)   
```
Workflow: read → split → loop → check → remove → join → write → verify.  

## Key Takeaways  

The lab combines foundational Python syntax with a security scenario. Keep the code, observed output, answers to reflection questions, and a short security relevance section in the GitHub file.  

## Skills Demonstrated  

- Python
- Cybersecurity automation
- Problem solving
- Code documentation 
