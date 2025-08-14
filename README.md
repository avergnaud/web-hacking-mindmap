
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
     - Enumeration in Authentication Forms - see [enumerationbruteforce](https://tryhackme.com/room/enumerationbruteforce)
     - Exploiting Vulnerable Password Reset Logic - see [enumerationbruteforce](https://tryhackme.com/room/enumerationbruteforce)
     - waybackurls
   - bruteforce
     - ffuf
     - Exploiting HTTP Basic Authentication - see [enumerationbruteforce](https://tryhackme.com/room/enumerationbruteforce)
   - logic flaw
   - cookie tampering
     - [https://crackstation.net](https://crackstation.net)
   - JWT - see [jwtsecurity](https://tryhackme.com/room/jwtsecurity)
     - Sensitive Information Disclosure
     - Signature Validation Mistakes
     - JWT Lifetimes
     - Cross-Service Relay Attacks
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
   - [https://github.com/t3l3machus/toxssin](https://github.com/t3l3machus/toxssin)
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

# access control

![access control](./Access-Control-vaulnerabilites.png?raw=true)

# Tools for Web Application Pentesting

![recon tools](./recon_tools.jpg?raw=true)

## final recon

[https://hakin9.org/final-recon-osint-tool-for-all-in-one-web-reconnaissance/](https://hakin9.org/final-recon-osint-tool-for-all-in-one-web-reconnaissance/)

[https://github.com/thewhiteh4t/FinalRecon](https://github.com/thewhiteh4t/FinalRecon)

## rekono

[https://securityonline.info/rekono-execute-complete-pentesting-processes/](https://securityonline.info/rekono-execute-complete-pentesting-processes/)

# Hacking articles 

## Web App Pentest

![hacking articles](./hacking-articles-mindmap.png?raw=true)

## Web application hacking

![hacking articles 2](./hacking-articles-webapp-hacking.png?raw=true)

# 0xshahriar web hacking mindmap

![0xshahriar](./Pentesting_Mind_Map_0xshahriar.png?raw=true)

# hakluke

[https://labs.detectify.com/2022/05/16/how-to-hack-web-applications/](https://labs.detectify.com/2022/05/16/how-to-hack-web-applications/)

[https://labs.detectify.com/2022/08/05/how-to-hack-web-applications-in-2022/](https://labs.detectify.com/2022/08/05/how-to-hack-web-applications-in-2022/)

# infrastructure

## DNS



# theCyberGuy recon mind map

![recon map](./theCyberGuy_Recon_V1.0.png?raw=true)

[https://github.com/Cyber-Guy1/theCyberGuy_Recon_V1.0](https://github.com/Cyber-Guy1/theCyberGuy_Recon_V1.0)
