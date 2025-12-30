# Bandit Level 28 → 29

## Goal:
Clone the remote Git repository using the Bandit28 password and find the password for the next level.

## Process:

1. Clone the Git repo through SSH on port 2220:

   `git clone ssh://bandit28-git@bandit.labs.overthewire.org:2220/home/bandit28-git/repo`

2. Enter Bandit28 password when prompted.
 
3. Move into the cloned repository:

  ` cd repo`

4. List files to inspect contents:

   `ls`

5. Read the file that stores the password:

   `cat README.md`

6. If password is not visible directly, check commit history:

    `git log -p`

7. Look for password hidden or changed in older commits.


## Password Found:

   4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7


## Screenshot:
   
   screenshots/Level28-29.png


## Notes:
 
-Learned how to clone Git repositories over SSH using a custom port.

-Learned to inspect commit history when data is modified or hidden.
