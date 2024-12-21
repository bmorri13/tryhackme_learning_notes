# Advent of Cyber 2024

## Reverse Engineering

- Went over basics of malicous binaries such as multi-stage binaries
    - Stage 1 - Dropper: lightweight, basic binary responsible for actions such as enumerating the operating system to see if the payload will work. Once certain conditions are verified, the binary will download the second - much more malicious - binary from the attacker's infrastructure.
    - Stage 2 - Payload: Binary is the "meat and bones" of the attack. For example, in the event of ransomware, this payload will encrypt and exfiltrate the data.
- IDA - used to guess what was ran in assembly to recreate the C program
- PEStudio - software designed to investigate potentially malicious files and extract information from them without execution
- ILSpy - Used to decomplie .net code for us to review what the app code is doing

### Room Example

- Using ILSpy, we reviewed the code of the initial malware app to see what the code was doing if it were to be executed.
    - We found the address where it would reach out to in order to download the second stage malware
- Visited the link to download the second stage malware, threw that into ILSpy in order to again review the code to find out the remianing flags for the lab
