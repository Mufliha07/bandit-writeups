# Bandit Level 17 → 18

## Goal:
Find the password for the next level by identifying the only line that was changed between passwords.old and passwords.new.

## Login:
Logged into Bandit17 using credentials from the previous level.

## Commands used & Purpose:

ls  → Listed the files in the home directory to locate passwords.old and passwords.new

diff passwords.old passwords.new 
→ Compared both files and identified the only modified line which contains the next password

## Password found:
x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO

## Screenshot:
screenshots/Level17-18.png

## Notes:
This level teaches comparing two files using diff and extracting the only changed line to find the password for the next level.
