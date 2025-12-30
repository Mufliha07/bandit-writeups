# Bandit Level 23 → 24

## Goal
Inspect the cron job and execute a custom shell script to retrieve the next level password stored in /tmp/.

----

## Process

1.`ls /etc/cron.d/` 
→ Listed cron configuration files.

2. `cat /etc/cron.d/cronjob_bandit24` 
→ Read which script runs automatically.

3. `cat /usr/bin/cronjob_bandit24.sh` 
→ Inspected the cron‑executed script.

4. `mkdir /tmp/bn23-24`
→ Created a temporary working directory.

5. `cd /tmp/bn23-24` 
→ Moved into the created directory.

6. Created script.sh using nano:
    #!/bin/bash
    cat /etc/bandit_pass/bandit24 > /tmp/bn23-24/pass
→ Script reads Bandit24 password and stores it in /tmp/bn23-24/pass.

7. `chmod 777 script.sh` 
→ Gave full execute permission to the script.

8. `cp script.sh /var/spool/bandit24/foo/`
→ Copied script into cron execution directory.

9. `ls -alps /tmp/bn23-24`
→ Verified file creation.

10. `cat /tmp/bn23-24/pass`
→ Read the extracted password.

---

## Password Found
gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8

----

## Screenshot 
 screenshots/Level23-24_(1).png
 
 screenshots/Level23-24_(2).png
 
----

## Notes

- Learned how cron executes scripts automatically.
- Learned creating and using a custom shell script to extract passwords.

