# Create More Functions  

## Objective  
Analyze failed-login data with built-ins, parameters, return values, and ratios.  

## Core Code and Explanation  

script:
```python 
failed_login_list = [85, 88, 90, 91, 92, 99, 101, 105, 108, 119, 223, 264] 
  print(sorted(failed_login_list))
  print(max(failed_login_list))
def analyze_logins(username, current_day_logins, average_day_logins):
  login_ratio = current_day_logins / average_day_logins
  return login_ratio

login_analysis = analyze_logins("ejones", 9, 3)
if login_analysis >= 3:
   print("Alert: login activity requires investigation") ```

The values 223 and 264 are notable outliers relative to the remaining list.  

## Key Takeaways  

The lab combines foundational Python syntax with a security scenario. Keep the code, observed output, answers to reflection questions, and a short security relevance section in the GitHub file.  

## Skills Demonstrated  

- Python
- Cybersecurity automation
- Problem solving
- Code documentation 

```python
failed_login_list = [85, 88, 90, 91, 92, 99, 101, 105, 108, 119, 223, 264] 
  print(sorted(failed_login_list))
  print(max(failed_login_list))
def analyze_logins(username, current_day_logins, average_day_logins):
  login_ratio = current_day_logins / average_day_logins
  return login_ratio

login_analysis = analyze_logins("ejones", 9, 3)
if login_analysis >= 3:
   print("Alert: login activity requires investigation") ```





