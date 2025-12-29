# Bandit Level 9 → 10

**Goal:**
Find password stored inside data.txt next to a line containing = symbol, by extracting readable strings.

**Login:**
Logged into Bandit9 using previous level password.

**Commands used:**
ls                            → List files
strings data.txt | grep "="   → Extracted readable strings and found password

**Password found:**
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

**Screenshot:**
see ```screenshots/Level09-10.png```

**Notes:**
This level teaches extracting readable text from binary files using strings and searching using grep.
