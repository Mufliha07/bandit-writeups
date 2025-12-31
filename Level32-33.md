# Bandit Level 32 → 33

## Goal:
Escape the uppercase shell and retrieve the password for the next level.

## Solution:

1. Escape the restricted uppercase shell by spawning the default system shell:

   `$0`

2. Read the password file for Bandit33:

   `cat /etc/bandit_pass/bandit33`

## Password Found:
 
   tQdtbs5D5i2vJwkO8mEyYEyTL8izoeJ0

## Screenshot:

screenshots/Level32-33.png

## Notes:

   Escaped the uppercase shell using $0 to launch Bash and accessed the password file directly.
