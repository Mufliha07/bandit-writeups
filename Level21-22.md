# Bandit Level 21 → 22

## Goal:
Identify the cron job for Bandit22, read the executed script, and retrieve the password created in /tmp/.

## Process:

1. Navigate to the cron configuration directory:
   cd /etc/cron.d/

2. List all cron jobs:
   ls

3. Read the cron job for Bandit22:
   cat cronjob_bandit22

4. Read the script executed by the cron job:
   cat /usr/bin/cronjob_bandit22.sh

5. Check and read the password file generated in /tmp/:
   cat /tmp/t706lds9S0RqQh9aMcz6ShpAoZKF7fgv

## Password Found:
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q

## Screenshot:
screenshots/Level21-22.png

## Notes:
- This level teaches inspecting cron jobs and understanding how automated scripts can generate temporary password files.
- The password is automatically written by the cron job; no manual execution is required.
