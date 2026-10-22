# Use Regular Expressions to Find Patterns

## Objective

Extract device identifiers and IP-like patterns from log text.

## Core Code and Explanation
```python
import re
target_pattern = r"r15\w+"
matching_devices = re.findall(target_pattern, devices)
pattern = r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}"
valid_ip_addresses = re.findall(pattern, log_file)
for address in valid_ip_addresses:
    if address in flagged_addresses:
        print(address, "has been flagged for further analysis")
    else:
        print(address, "does not require further analysis")
```
Note: this regex limits segment length but does not enforce IPv4 values between 0 and 255.

## Key Takeaways

The lab combines foundational Python syntax with a security scenario. Keep the code, observed output, answers to reflection questions, and a short security relevance section in the GitHub file.

## Skills Demonstrated
- Python
- Cybersecurity automation
- Problem solving
- Code documentation 
