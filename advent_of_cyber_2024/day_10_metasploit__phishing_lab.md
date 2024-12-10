# Advent of Cyber 2024

## Metasplot - Phishing Lab

- Reviewed using Metasplot's meterpreter module to create a word doc to include a macro to exploit a reverse shell
- Sent the email to a fake end user and tested results after reverse shell is established

### Room Example
- First created a malicious word doc with a macro to establish a reverse shell when started using meterpreter
- Set up a listener for a reverse shell with meterpreter
- Sent a phishing email with the malicous word doc included, waited for user to open it. Once opened, established the reverse shell and we navigated to find the flag on the admins desktop.
