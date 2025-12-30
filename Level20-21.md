## Level: Bandit 20 → 21

## Goal:
Use the setuid binary suconnect to retrieve the password for the next level by verifying the current level password through a netcat listener using SSL/TLS.

## Steps:

1. Identify the current password for Bandit20:
   cat /etc/bandit_pass/bandit20

2. Open a listener in a second terminal:
   nc -lp 9999

3. In the first terminal, connect using the setuid binary:
   ./suconnect 9999

4. Send the Bandit20 password in the listener terminal.

5. If the password matches, suconnect returns the next level password.

Result:
Password verified successfully and next password received.

## Password for Level 21:
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

## Screenshot:
screenshots/Level20-21.png

## Notes:
- Only one port listener returns the next password; others echo back the input.
- This level demonstrates inter-terminal communication using a setuid binary with network validation.
