**Bandit Level 1 → 2**

**Goal:**
Find the password stored in a file named - located in the home directory.

**Login:**
Logged into Bandit1 using the previous level password.

**Commands used:**
```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220 → Login to server using SSH on port 2220
ls -la                                          → List all files including special/hidden names
cat ./-                                         → Open the file - safely using ./ notation (to avoid command confusion)
```
**Password found:**
263JGJPfgU6LtdEvgfWU1XP5yac29mFx

**Screenshot:**
screenshots/Level01-02.png

**Notes:**
This level teaches how to read files that have unusual names like - using ./-.
