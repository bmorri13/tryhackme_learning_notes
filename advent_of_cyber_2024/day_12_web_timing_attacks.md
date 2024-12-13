# Advent of Cyber 2024

## Web Timing Attacks - Exploiting race condiitons with HTTP2

- Timing Attacks
    - Information Disclosures
    - Race Conditions
- TLDR When an app is set up you can take advantage of a race condiiton where you may try to send multiple requests to get around the backend processes such as quering a DB to see if funds exist before sending.
    - This is also big in web3 code as you have to account for this or you can have accounts / wallets drained easily.

### Room Example
- Tested with Burp suite sending multiple requests to get around the backend processes on the site force by senindg grouip requests in parallel to cause a race condition on the amount of money an account has and send it into the negative
