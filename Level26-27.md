# Bandit Level 26 → 27

## Goal:
Run the bandit27-do setuid binary to read the password for Bandit27.

## Login:
Logged into Bandit26 using the shell escaped from the previous level.

## Commands used:
`ssh bandit26@bandit.labs.overthewire.org -p 2220` → Login to the server using SSH 

`ls`                                               → List files and find the bandit27-do binary 

`./bandit27-do`                                    → Execute the setuid program to check how it works

`./bandit27-do cat /etc/bandit_pass/bandit27`      → Use the binary to run cat as Bandit27 and read the password file


## Password Found:
upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB

## Screenshot:
screenshots/Level26-27.png

## Notes:
- bandit27-do is a special binary that lets us run commands as Bandit27.
- We used it to run cat with higher privileges to read the password file.
- Learned how setuid programs help access restricted files safely in this game.
