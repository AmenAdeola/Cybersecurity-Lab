# Work with Strings in Python

## Objective

Convert, measure, concatenate, index, slice, and search strings.

## Core Code and Explanation

```python
employee_id = 4186
 employee_id = str(employee_id)
 if len(employee_id) < 5:
     employee_id = "E" + employee_id

device_id = "r262c36"
print(device_id[3])
print(device_id[0:3])

url = "https://exampleURL1.com"
ind = url.index(".com")
print(url[0:8])
print(url[8:ind]) print(url[ind:ind+4])
```
Key concepts:
`str()`, `len()`, concatenation, indexing, slicing, and `.index()`.

## Key Takeaways

The lab combines foundational Python syntax with a security scenario. Keep the code, observed output, answers to reflection questions, and a short security relevance section in the GitHub file.

## Skills Demonstrated

- Python
- Cybersecurity automation
- Problem solving
- Code documentation 
