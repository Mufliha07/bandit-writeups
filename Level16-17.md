# Bandit Level 16 → 17

**Goal:**
Find the only port in the range 31000–32000 that speaks SSL/TLS, submit the current level password, receive the RSA private key, and use it to log into Bandit17.

**Login:**
Logged into Bandit16 using the password obtained from Level 15 → 16.

**Commands used & Purpose:**

```nmap localhost -p 31000-32000```
→ Scanned localhost to find which ports have a server listening

```ncat --ssl localhost 31046```
→ Tried SSL connection but got input/output error

```ncat --ssl localhost 31518```
→ Port echoed back input, so not the correct server

```ncat --ssl localhost 31790```
→ Submitted current level password, got response "Correct!" and received RSA private key

exit  
→ Exited from Bandit16 server back to local machine

```echo "<PASTE_RSA_PRIVATE_KEY_HERE>" > bandit16-17```
→ Saved copied RSA key into a local file

```chmod 700 bandit16-17```
→ Gave secure permission to the key file

```ssh bandit17@bandit.labs.overthewire.org -p 2220 -i bandit16-17```
→ Logged into Bandit17 using the extracted RSA private key

**Password found:**
(No password was obtained here, only RSA private key was received)

**Screenshot:**
screenshots/Level16-17_step1.png
screenshots/Level16-17_step2.png
screenshots/Level16-17_step3-final.png

**Notes:**
This level teaches port scanning using nmap, identifying SSL/TLS services, testing ports using ncat with SSL, extracting an RSA private key, storing it securely,
giving proper permissions, and authenticating into another SSH user using -i flag.
