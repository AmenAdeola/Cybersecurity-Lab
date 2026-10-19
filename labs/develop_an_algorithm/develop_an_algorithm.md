# Develop an Algorithm  

## Objective  

Verify approved usernames and assigned device IDs.  

## Core Code and Explanation  

```python def login(username, device_id):     approved_users = ["elarson", "bmoreno", "sgilmore"]     approved_devices = ["8rp2k75", "h1o5so1", "4n482ts"]      if username in approved_users:         index = approved_users.index(username)         if device_id == approved_devices[index]:             print("Approved user and assigned device")         else:             print("Approved user, but device is not assigned to this user")     else:         print("User is not approved") ```  

Synchronized lists use the same index to associate related usernames and devices.  

## Key Takeaways  

The lab combines foundational Python syntax with a security scenario. Keep the code, observed output, answers to reflection questions, and a short security relevance section in the GitHub file.  

## Skills Demonstrated  

- Python
- Cybersecurity automation
- Problem solving
- Code documentation 
