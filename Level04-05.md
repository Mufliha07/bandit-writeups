# Bandit Level 4 → 5

**Goal:** Find the only human‑readable file inside inhere directory and read the password.

**Login:** Used the password from Level 3 → 4.

**Commands used:**
```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
ls
cd inhere
ls -la
file ./*
cat ./-file07
```
**Password Found:** 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

**Screenshot:** see screenshot/Level04-05.png
