# Create Conditional Statements  

## Objective

Automate decisions about operating-system updates, user approval, and login timing.  

## Core Code and Explanation  
script:
if system == "OS 2": 
  print("no update needed") 
elif system == "OS 1" or system == "OS 3":     
  print("update needed")  
if username in approved_list and organization_hours:    
  print("Approved login") 
else:    
  print("Username not approved or login occurred outside organization hours") 
  
  Key concepts: if, elif, else, and, or, and in. 
  
## Key Takeaways  

The lab combines foundational Python syntax with a security scenario. Keep the code, observed output, answers to reflection questions, and a short security relevance section in the GitHub file.  

## Skills Demonstrated 

- Python
- Cybersecurity automation
- Problem solving
- Code documentation 
