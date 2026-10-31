# Python Debugging  

## Error Types  
| Error | Meaning | Example |
|---|---|---|
| SyntaxError | Invalid syntax | Missing colon |
| IndentationError | Incorrect indentation | Block not aligned |
| TabError | Mixed tabs and spaces | Inconsistent indentation |
| NameError | Unknown name | Misspelled variable |
| TypeError | Incompatible data type | Writing a list directly to a file |
| IndexError | Index outside valid range | `items[5]` with five items |
| ValueError | Invalid value | `.remove()` for absent value |
| AttributeError | Unsupported method | Calling `.split()` on the wrong object |
| Logic error | Code runs but result is wrong | Incorrect comparison operator |



## Debugging Workflow

1. Read the full error message.
2. Identify the line number.
3. Reproduce the problem with the smallest input.
4. Print variables and types.
5. Verify assumptions and expected output.
6. Correct one issue at a time.
7. Rerun the test.
8. Add a test to prevent recurrence.
9. 
  
## Useful Techniques
```python

print(variable) print(type(variable)) print(len(items))
```
 Use four spaces for indentation and meaningful variable names. 
