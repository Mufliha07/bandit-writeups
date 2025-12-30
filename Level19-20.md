# Bandit Level 19 → 20

## Goal:
Use the setuid binary bandit20-do to execute commands as Bandit20 and retrieve the password stored in /etc/bandit_pass/bandit20.

## Login:
Logged into Bandit19 using the password from the previous level.

## Commands used & Purpose:

ls -l  
→ Listed files to locate the setuid binary in the home directory

./bandit20-do  
→ Executed the setuid binary without arguments to understand how to use it

./bandit20-do cat /etc/bandit_pass/bandit20  
→ Used the binary to run cat as Bandit20 user and read the next level password file

## Password found:
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO

## Screenshot:
screenshots/Level19-20.png

## Notes:
This level teaches how to leverage a setuid binary to run commands as another user and access restricted password files securely.
