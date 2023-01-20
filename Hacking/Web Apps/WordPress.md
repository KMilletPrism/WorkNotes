# Attacking Wordpress Applications
## Resources
### HackTricks Page
https://book.hacktricks.xyz/network-services-pentesting/pentesting-web/wordpress

## WP Scan
Basic WPScan usage looks like the following
`wpscan --url https://target-domain.com`

Useful flags
`--random-user-agent` - Randomises the user agent after every request to avoid being blocked.

`--api-token` - Get your API token from https://wpscan.com/profile (Login required) and your scan can include specific vulnerabilities for out of date plugins etc. Without the API key vulnerabilities will not be included