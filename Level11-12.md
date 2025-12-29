# Bandit Level 11 → 12

**Goal:**
Decode ROT13 encoded content from data.txt and extract the password.

**Login:**
Logged into Bandit11 using previous level password.

**Commands used:**
```bash
ls                                           → Listed files in home directory  
cat data.txt                                 → Displayed encoded content  
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'    → Decoded ROT13 and revealed password  
```
**Password found:**
7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

**Screenshot:**
see ```screenshots/Level11-12.png```

**Notes:**
This level teaches decoding ROT13 using tr command in Linux.
