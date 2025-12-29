# Bandit Level 2 → 3

**Goal:**
Find the password stored in a file that has spaces in its name, located in the home directory.

**Login:**
Logged into Bandit2 using the previous level password.

**Commands used:**
```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220         → Login to server using SSH  
ls                                                      → List all files  
cat ./--spaces\ in\ this\ filename--                    → Read the file with spaces using quotes  
```

**Password found:**
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

**Screenshot:**
see ```screenshots/Level02-03.png```

**Notes:**
This level teaches reading files that contain spaces in their names using quotes.
