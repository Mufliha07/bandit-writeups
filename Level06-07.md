# Bandit Level 6 → 7

**Goal:**
Find password stored in a file somewhere on the server with these properties:
- Owned by user bandit7
- Owned by group bandit6
- 33 bytes in size

**Login:**
Logged into Bandit6 using previous level password.

**Commands used:**
```bash
find / -type f -size 33c -group bandit6 -user bandit7 2>/dev/null   → Searched for matching file
cat /var/lib/dpkg/info/bandit7.password                             → Read the file and copied password
```
**Password found:**
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

**Screenshot:**
see ```screenshots/Level06-07.png```

**Notes:**
This level teaches searching system files using ownership, group, and size filters with find command.
