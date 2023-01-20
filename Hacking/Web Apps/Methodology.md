## Every Test Scans

- SSL Scan - `sslscan <url>`
- NMap scan of host - `nmap -sC -sV <url>`
- WAF scan - `wafw00f <url>`
- Directory scan - `dirb <url> <wordlist>`
- Nessus scan of target using GUI
- Nikto web vulnerability scanner

## Every Test Checks
- Does the application have a strong password policy?
- Are there missing security headers. Check using [Security Headers Checker](https://securityheaders.com) and BurpSuite. The security headers site also has a Python  script available [here](https://github.com/juerkkil/securityheaders)
- Check for interesting file types using Google - `site: <domain-name> filetype: docx OR filetype: pdf OR filetype: pptx`
- Is there an account lockout mechanism? How many attempts does it allow?
- Decode auth tokens to see if sensitive data has been included in them.
- Subdomain enumeration

## OSINT Checks
- Does the site have source code on GitHub?
- Are there older versions of the site on the Internet Archive?
- Can you find credentials using services like Dehashed?

## Vulnerability Checklist
- XSS
- SSTI
- SQLi
- CSRF
- XXE
- Broken access control / IDOR

## Specialty Areas

### Payment Systems
- Ensure caveats regarding third parties are included in the report. If changing data sent to third parties affects payment outcomes, we won't pick it up.

### Cloud Infrastructure
- Useful guides for testing Amazon cloud infrastructure: [S3 Bucket Testing](https://notes.offsec-journey.com/cloud-security-pentest/penetration-testing-aws-storage), [AWS Storage](https://notes.offsec-journey.com/cloud-security-pentest/penetration-testing-aws-storage)