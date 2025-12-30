**Goal:**
Extract the password hidden inside multiple compressed and encoded layers in data.txt.

**Login:**
Logged into bandit12 using the password obtained from the previous level.

**Commands used:**
```bash
mkdir /tmp/ban12-13             → Created a temporary working directory to safely process the file
cp data.txt /tmp/ban12-13       → Copied the encoded file into the temporary directory
cd /tmp/ban12-13                → Moved into the working directory
xxd -r data.txt > data.bin      → Decoded the hex dump back into its original binary form
file data.bin                   → Identified the file type to determine the next decompression method
mv data.bin data.gz             → Renamed the file to .gz format for gzip extraction
gzip -d data.gz                 → Decompressed the gzip layer
file <filename>                 → Checked the next layer file type
mv <filename> data.bz2          → Renamed the file to .bz2 format for bzip2 extraction
bzip2 -d data.bz2               → Decompressed the bzip2 layer
mv <filename> data.tar          → Renamed the file to .tar format for tar extraction
tar xf data.tar                 → Extracted the tar archive
cat <final file>                → Read the final human-readable file containing the password
```
**Password found:**
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

**Screenshots:**
```bash
screenshots/Level12-13_step1.png
screenshots/Level12-13_step2.png
screenshots/Level12-13_step3.png
screenshots/Level12-13_step4.png
screenshots/Level12-13_step5.png
screenshots/Level12-13_final.png
```
**Notes:**
This level teaches manual decoding of hex dumps and handling multiple compression layers to extract hidden data.
