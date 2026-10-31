# Python for Cybersecurity  

## Data Types  
| Type | Example | Use |
|---|---|---|
| string | `"analyst"` | Usernames, IPs, hashes |
| integer | `5` | Counts and thresholds |
| float | `3.5` | Ratios and measurements |
| Boolean | `True` | Status and conditions |
| list | `["ip1", "ip2"]` | Ordered mutable values |
| dictionary | `{"severity": "high"}` | Structured events |
| set | `{"hash1", "hash2"}` | Unique indicators |  


## Conditions  
```python
if severity == "high":
     print("Escalate")
 elif severity == "medium":
     print("Investigate")
 else:     print("Monitor")
```

## Loops  

```python
for ip in ip_addresses:
     if ip in allow_list:
         print("Allowed")
     else:
         print("Investigate")
```
## Functions
```python
def analyze_logins(current, average):
     return current / average
```
## Common Functions and Methods
`print()`, `type()`, `len()`, `min()`, `max()`, `sorted()`, `.upper()`, `.lower()`, `.index()`, `.append()`, `.remove()`, `.split()`, and `.join()`.  

## Regex
```python
import re
pattern = r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}"
addresses = re.findall(pattern, log_text)
```

## Security Uses  
- Parse logs
- Extract indicators
- Update allow lists
- Count events
- Identify patterns
- Automate repetitive checks
- Produce structured reports 
