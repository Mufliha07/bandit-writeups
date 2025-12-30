## Bandit Level 25 → 26

## Goal:
Login from Bandit25 → Bandit26 using the provided SSH private key, identify the restricted shell, and escape into a normal bash shell.

## Process:

1. Login to Bandit25 
   `ssh bandit25@bandit.labs.overthewire.org -p 2220`

2. List files and locate SSH key
   `ls -l`

3. Read the SSH private key
   `cat bandit26.sshkey`

4. Exit back to local machine
   `exit`

5. Save the copied key locally
   `echo "<PASTE_COPIED_KEY_HERE>" > /tmp/bandit25-26`

6. Give correct permissions to key file
   `chmod 700 /tmp/bandit25-26`

7. Login to bandit26 using SSH key
   `ssh bandit26@bandit.labs.overthewire.org -p 2220 -i /tmp/bandit25-26`

8. After login, the terminal open in s=a different shell(no bash), Resize terminal to very small size so it opens more pager mode,then break out using:
   `v` (pree v to enter vim)

9. Set vim shell, spawn bash shell
   ```
    :set shell=/bin/bash
    :shell
    ```

## Password Found:
No password is retrieved here. Only the SSH private key is obtained and used to login to Bandit26.

## Screenshot:
screenshots/Level25-26_(1).png
screenshots/Level25-26_(2).png

## Notes:
 Learned to escape restricted shells using vim shell spawn.
