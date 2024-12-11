# Advent of Cyber 2024

## OpSec - Operational Security

- Protecting your persona; / identifiable infomration with the goal to not allow yourself (or an attacker to be identified)

### Examples of Poor OPSEC

- Reusing usernames, email addresses, or account handles across multiple platforms. One might assume that anyone trying to cover their tracks would remove such obvious and incriminating information, but sometimes, it's due to vanity or simply forgetfulness.
  -Using identifiable metadata in code, documents, or images, which may reveal personal information like device names, GPS coordinates, or timestamps.
- Posting publicly on forums or GitHub (Like in this current scenario) with details that tie back to their real identity or reveal their location or habits.
- Failing to use a VPN or proxy while conducting malicious activities allows law enforcement to track their real IP address.

### Room Example

- Walked through downloading a malicious file example and using `file` & `exiftool` to view the malicious file's metadata information
- It was discovered that the 'bad' `somg.mp3` contains a powershell script and is actually a Windows shortcut filetype (e.g. `.lnk` file)
- Following the callback to downlaod the powershell script, you can see that there is a unique signature for `M.M.` in there which we then investigated in GitHub for code commits by that user. Their profile was found and in there you can see a .github config file that says who they are
