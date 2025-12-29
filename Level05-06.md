# Bandit Level 5 → 6

**Goal:**
Find password stored somewhere inside inhere directory with specific properties:
- Human readable
- 1033 bytes size
- Not executable

**Login:**
Used the password from Level 4 → 5.

**Commands used:**
```bash
cd inhere                                         → Entered the directory
ls -la                                            → Listed all files
find . -type f -size 1033c ! -executable          → Found matching readable file
cat ./maybehere07/.file2                        → Read file and copied password
```
**Password found:**
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

**Screenshot:**
see ```screenshots/Level05-06.png```

**Notes:**
This level teaches searching files based on size, readability, and permissions using find command.
