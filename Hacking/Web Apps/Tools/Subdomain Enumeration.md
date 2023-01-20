- Use `dnsrecon` to automate scanning DNS records with a wordlist
- Use `Sublist3r` (not built into Kali) to automate OSINT enumeration
- Use Ffuf to fuzz for subfdomains using the Host header. This checks virtual hosts on the webserver which may not have DNS records or turn up in OSINT checks. See examples below.

``` bash
user@machine$ ffuf -w /usr/share/wordlists/SecLists/Discovery/DNS/namelist.txt -H "Host: FUZZ.acmeitsupport.thm" -u http://MACHINE_IP
```

``` bash
user@machine$ ffuf -w /usr/share/wordlists/SecLists/Discovery/DNS/namelist.txt -H "Host: FUZZ.acmeitsupport.thm" -u http://MACHINE_IP -fs {size}
```

- You can also use manual OSINT tools. You can search for registered SSL certificates using [Certificate Search](https://crt.sh/). You can also use the *site:* filter on Google to include only results from a particular domain.