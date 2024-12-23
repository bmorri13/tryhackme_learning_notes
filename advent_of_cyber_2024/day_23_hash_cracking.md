# Advent of Cyber 2024

## Hash Cracking

- Going over identifying the hash type
    - Used sample python script
    - Also went over using name-that-hash (nth) can be installed on kali / ran via link pacakges
        - This is nice since it gives you the tools you can use to crack it
- Went over using john the ripper tool and the word list to crack the raw-shaw256 password
    - Went over to to also use the rule list for wordlist to check for variations of the password in the password list
```bash
john --format=raw-sha256 --wordlist=/usr/share/wordlists/rockyou.txt --rules=wordlist hash1.txt
```

### Room Example

- Used John the Ripper to crack the password via the wordlists and also used the tool via john to conver the pdf to get out the password hash, then we ran john with the word list to get out the password followed ten by making the pdf a text doc and then giving the the cracked password to the retrieve the final flag:

```bash
pdf2john.pl private.pdf > pdf.hash
john --rules=single --wordlist=wordlist.txt pdf.hash
pdftotext private.pdf  -upw M4y0rM41w4r3
```
