# Create Loops in Python  

## Objective 

Automate repeated connection messages, IP allow-list checks, and ID generation.

## Core Code and Explanation  

```python 
for i in range(3):     
  print("Connection could not be established.")  
for ip in ip_addresses:     
  if ip in allow_list:        
    print("IP address is allowed")     
  else:        
    print("IP address is not allowed. Further investigation required.")        
    break  
i = 5000 
while i <= 5150:     
  print(i)     
    i += 5 
     ```
  Key concepts: for, while, range(), counters, membership, and break.  
    
  ## Key Takeaways  
 The lab combines foundational Python syntax with a security scenario. Keep the code, observed output, answers to reflection questions, and a short security relevance section in the GitHub file. 
  
  ## Skills Demonstrated  
  
  - Python
  - Cybersecurity automation
  - Problem solving
  - Code documentation 
