# Advent of Cyber 2024

## Certificate Mismanagement

- Reviewed what makes up a certificate, what CA is (e.g. digicert), Self Signed vs Trusted CA's and where / when they would be used

### Room Example

- Tested accessing the insurcure site with a self-signed cert
- By doing so, we tested setting up a proxy to intercept the user traffic that we simulated with a shell script
- From there, we were able to see the user credentials and use those to compromise the accounts to get the necessary flags
