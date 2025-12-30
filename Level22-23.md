# Bandit Level 22 → 23

## Goal:
Inspect cron job in /etc/cron.d/ and identify the script/command executed automatically for the next level.

## Process:

1. Navigate to the cron configuration directory:
   cd /etc/cron.d/

2. List all cron jobs:
   ```ls```

3. Read the cron job for Bandit23:
   ```cat cronjob_bandit23```

4. Read the script executed by the cron job:
   ```cat /usr/bin/cronjob_23.sh```

5. Reproduce the hashed filename created by the cron script:
   ```echo I am user bandit23 | md5sum | cut -d ' ' -f1```

6. Read the password stored in the generated hashed file inside /tmp/:
   ```cat /tmp/8ca319486bfbbc3663ea0fbe81326349```

## Password Found:
0Zf11ioIjMVN551jX3CmStKLYqjk54Ga

## Screenshot:
screenshots/Level22-23.png

## Notes:
- Learned how cron scripts create dynamic filenames using hashes.
- Learned to manually reproduce the MD5 hash to locate and read stored passwords.
