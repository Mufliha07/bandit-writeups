# Bandit Level 10 → 11

**Goal:**
Decode the Base64 content from data.txt and extract the password for Level 11.

**Login:**
Logged into Bandit10 using previous level password.

**Commands used:**
```bash
ls                 → Listed files in home directory
cat data.txt       → Viewed Base64 encoded content
base64 -d data.txt → Decoded and extracted password
```
**Password found:**
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

**Screenshot:**
see ```screenshots/Level10-11.png```

**Notes:**
This level teaches decoding Base64 using base64 -d.
