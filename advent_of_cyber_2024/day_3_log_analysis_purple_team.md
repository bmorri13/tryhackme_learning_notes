# Advent of Cyber 2024

## Log Analysis and Red Team items (Purple teaming)

- Goes over some log analsys initiall
- Reviews:
    - **RCE** - Remote Code Execution - Uploading a script that the server runs gives the attacker control over it.
        - When an attacker finds a way to run their own code on a system
    - **XSS** - Cross Site Scripting - Uploading an HTML file that contains an XSS code which will steal a cookie and send it back to the attacker's server.

### Room Example
- Updated /etc/hosts file to include path to the frostypines site
- Queried ELK for finding out what RCE file is being executed from the images directory
- Found the client ip who is doing the actions
- Used default credentials to gain admin access with email
- Upload script for RCE by creating a new room and uploading that script as a room image
- Navigated to the script file and we can then run commands to ls and cat the flag.txt file
