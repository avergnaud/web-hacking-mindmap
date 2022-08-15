
# OWASP testing guide

[https://owasp.org/www-project-web-security-testing-guide/latest/](https://owasp.org/www-project-web-security-testing-guide/latest/)

# mind map - web hacking

- walking an application
   - view source
   - inspector
   - debugger
   - network
- content discovery
   - manual discovery
      - robots.txt
      - favicon
      - sitemap
      - HTTP headers
      - framework stack
   - OSINT
     - Google hacking / dorking
     - Wappalyzer
     - Wayback machine
     - GitHub
     - S3 buckets
   - automated discovery
     - word lists
       - SecLists
     - automation tools
       - ffuf
       - dirb
       - gobuster
       - [nuclei](https://nuclei.projectdiscovery.io/nuclei/get-started/)
- subdomain enumeration
   - bruteforce
     - dnsrecon
   - OSINT
     - Certificate Transparency (CT) logs
     - Search engines / Google hacking "-site:..."
     - sublist3r
   - virtual hosts
     - ffuf
- authentication bypass
   - username enumeration
     - ffuf
   - bruteforce
     - ffuf
   - logic flaw
   - cookie tampering
     - [https://crackstation.net](https://crackstation.net)
- Insecure Direct Object Reference
   - ids
     - base64
     - hashed
     - unpredictable
- File Inclusion
   - PHP [file_get_contents](https://www.php.net/manual/fr/function.file-get-contents.php) like
   - Local File Inclusion
     - PHP include, require ($_GET["..."])
     - ../
     - null byte
     - /etc/passwd/.
     - ....//....//etc/passwd
   - Remote File Inclusion
- Server Side Request Forgery
   - Blind SSRF. [https://requestbin.com/](https://requestbin.com/)
- Cross-site scripting
   - Reflected XSS
   - Stored XSS
   - DOM based XSS
   - Blind XSS
     - [https://xsshunter.com/](https://xsshunter.com/)
- Command injection
   - command-injection-payload-list
- SQL injection
   - In-Band SQL injection
   - Error-Based SQL injection
   - Union-Based SQL injection
   - Blind SQLi
     - Authentication Bypass
     - Boolean based
     - Time based
   - Out-of-Band SQLi  

# mind map - access control

![access control](./Access-Control-vaulnerabilites.png?raw=true)

## infrastructure

### DNS



# theCyberGuy recon mind map

![recon map](./theCyberGuy_Recon_V1.0.png?raw=true)

[https://github.com/Cyber-Guy1/theCyberGuy_Recon_V1.0](https://github.com/Cyber-Guy1/theCyberGuy_Recon_V1.0)