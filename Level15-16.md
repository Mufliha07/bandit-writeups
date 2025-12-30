# Bandit Level 15 → 16

**Goal:**
Retrieve the password for Level 16 by submitting the current level password to a service running on localhost port 30001 using SSL/TLS.

**Login:**
Logged into Bandit15 using the password obtained from Level14-15.

**Process:**

1. Connect securely to the service on localhost port 30001 using ncat with SSL:
  ```ncat --ssl localhost 30001```

2. Submit the current level password when prompted.

3. The service checks the password and responds with the password for Level16.

**Password Found:**
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

**Screenshot:**
```screenshots/Level15-16_final.png```

**Notes:**
This level teaches interacting with an SSL/TLS-encrypted service using ncat and submitting the current level password to retrieve the next password.
