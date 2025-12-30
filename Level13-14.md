**Level:** Bandit 13 → 14

**Goal:**
Use the private SSH key from Bandit13 to log into Bandit14 and retrieve the next password.

**Process:**

Login to Bandit13 server:
ssh bandit13@bandit.labs.overthewire.org -p 2220

List files to locate the SSH private key:
ls -l

Read the contents of the private key:
cat sshkey.private

Exit from Bandit13 back to local machine:
exit

Save the copied SSH key into a new file locally using echo:
echo "<PASTE_COPIED_KEY_HERE>" > bandit13-14

Give proper file permission for the SSH key:
chmod 700 bandit13-14

Login to Bandit14 using the saved private key:
ssh bandit14@bandit.labs.overthewire.org -p 2220 -i bandit13-14

Read the password for the next level:
cat /etc/bandit_pass/bandit14

**Password Found:**
This level does not contain a password. The SSH key was extracted and used to login to Bandit14, where the next level password was retrieved.

**Screenshot:**
```
screenshots/Level13-14-step1.png
screenshots/Level13-14-step2.png
screenshots/Level13-14-step3.png
screenshots/Level13-14-step4_final.png
```
**Notes:**
This level teaches how to extract SSH private keys and use them securely on a local machine to authenticate into another SSH user.
