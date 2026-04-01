# # XSS Lab – Gamespot

## Purpose
This repository documents a Cross-Site Scripting (XSS) vulnerability discovered on Gamespot as part of a cybersecurity learning exercise in a safe lab environment.

## Tools Used
- Kali Linux (VM)
- Firefox
- Burp Suite (for testing payloads)

## Vulnerability Type
- **Reflected XSS**  
The vulnerability occurs when user input is not properly sanitized and is reflected back to the page, allowing execution of arbitrary JavaScript.

## Steps to Reproduce (Safe)
1. Open the target page on Gamespot.
2. Enter a payload like: 
   "><script>alert(1)</script>
   As well as ![80731](https://github.com/user-attachments/assets/24761ab0-83e2-476f-9b2c-b95e116abe85)

   %3Cscript%3Ealert(1)%3C/script%3E
   These will send alerts just as that from the screenshot I posted.
 ##  Mitigation Recommendations
1, Implement proper input validation and sanitization
2, Encode output before rendering in HTML
3, Use Content Security Policy (CSP)
4, Avoid directly reflecting user input in responses
##  Disclaimer 
This project is for educational practical purposes only. Testing was done in a controlled environment. No real users or sensitive data were targeted.
## Cyber security student documenting Labs and vulnerability testing.
