# Bandit Level 18 → 19

## Goal:
Read the password from readme even though .bashrc forces logout on interactive SSH login.

## Login:
Attempted to login to Bandit18, but got logged out due to modified .bashrc.

## Commands used & Purpose:

ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"  
→ Logged in and executed cat readme directly without entering an interactive shell, bypassing the forced logout.

## Password found:
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8

## Screenshot:
screenshots/Level18-19.png

## Notes:
This level teaches how to execute commands remotely over SSH without spawning a shell, preventing .bashrc from triggering logout.
