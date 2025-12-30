# Bandit Level 27 → 28

## Goal:
Clone the remote Git repository using Bandit27 password, explore the files, and retrieve the password for the next level (Bandit28).

## Process:

1. Clone the Git repo through SSH on port 2220:

   `git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo`

2. Move into the cloned repository:

  ` cd repo`

3. List files to inspect contents:

   `ls`

4. Read the file that stores the password:

   `cat README`

## Password Found:
Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN

## Screenshot:
screenshots/Level27-28.png

## Notes:
- Git repositories can store sensitive data inside files or commit history.
- SSH cloning requires the same password as the current level.
- Learned how to clone and explore a remote Git repository from terminal.
