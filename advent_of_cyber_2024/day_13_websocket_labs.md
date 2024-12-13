# Advent of Cyber 2024

## Websocket Vulnerabilites and Manipulation Lab

- WebSockets let your browser and the server keep a constant line of communication open
- Used in
    - Chat apps
    - Games
    - Live feeds when you need real time data flow

- WebSocket Vulnerabilities
    - Weak Authentication and Authorisation
    - Message Tampering
    - Cross-Site WebSocket Hijacking (CSWSH)
    - Denial of Service (DoS)

- Risks of Websocket manipulation
    - Doing Things Without Permission
    - Gaining Extra Privileges
    - Messing Up Data
    - Crashing the System

### Room Example
- Used Burp tot est out capturing websocket traffic and modified the user ID value before forwarding th request to reveal the necessary flag
    - Used this to manupuate the message being sent to mimic messaging from another user to extract the flag
