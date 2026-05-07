# Time-Based User Enumeration PoC

This script is a Proof of Concept (PoC) designed for CTF challenges to demonstrate **Time-Based Side-Channel Attacks** on login endpoints. 

### How it works
The script measures the response time of the server for different usernames. If the server takes longer to process a request (e.g., due to password hashing for an existing user), the script identifies it as a potential valid username.

### Usage
```bash
python3 exploit.py -t http://<TARGET_IP>/api/user/login -w /path/to/wordlist.txt
