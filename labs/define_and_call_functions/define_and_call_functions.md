# Define and Call Functions  

## Objective  

Create reusable alert and list-processing functions.  

## Core Code and Explanation  
```python 
def alert():
     for i in range(3):
      print("Potential security issue. Investigate further.")

alert()
def list_to_string():
    username_list = ["elarson", "bmoreno", "tshah"]
    result = ""
    for username in username_list:
      result = result + username + ", "
    print(result)

list_to_string()
```
Functions reduce duplication, improve organization, and support automation.

## Key Takeaways  The lab combines foundational Python syntax with a security scenario. Keep the code, observed output, answers to reflection questions, and a short security relevance section in the GitHub file.  


## Skills Demonstrated  

- Python
- Cybersecurity automation
- Problem solving
- Code documentation 
