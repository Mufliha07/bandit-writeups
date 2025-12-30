**Level:** Bandit 14 → 15

**Goal:**
Retrieve the password for Level 15 by submitting the current level password to port 30000 running on localhost.

**Login:**
Logged into Bandit14 using the shhkey from previous level.

**Process:**

1. Submit the current level password to localhost port 30000 using netcat:
   nc localhost 30000

2. After sending the password, the service responds with the password for the next level.

**Password Found:**
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo

**Screenshot:**
```screenshots/Level14‑15.png```

**Notes:**
This level teaches using nc (netcat) to interact with a service running on a specific port and retrieving data by submitting input.
