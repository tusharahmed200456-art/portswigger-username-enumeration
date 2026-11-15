# portswigger-username-enumeration
PortSwigger Apprentice lab – Username Enumeration using Burp Suit
# Username Enumeration via Different Responses

![PortSwigger](https://img.shields.io/badge/Platform-PortSwigger-orange)
![Level](https://img.shields.io/badge/Level-Apprentice-blue)
![Status](https://img.shields.io/badge/Status-Solved-success)

## Lab Overview
This lab demonstrates username enumeration through different login responses and password brute-force attacks.

**Platform:** PortSwigger Web Security Academy

**Category:** Authentication

**Difficulty:** Apprentice

**Status:** Successfully Solved

## Tools Used
- Burp Suite Professional
- Burp Proxy
- Burp Intruder

## Objectives
- Identify a valid username.
- Perform password testing using the provided candidate password list.
- Successfully authenticate and access the account page.

## Methodology

### 1. Request Interception
Intercepted the login request using Burp Suite Proxy and sent it to Intruder.

### 2. Username Enumeration
- Selected Sniper attack type.
- Configured the username parameter as the payload position.
- Loaded the candidate usernames wordlist.
- Analyzed HTTP responses and response lengths.
- Identified a valid username.

### 3. Password Testing
- Kept the valid username fixed.
- Configured the password parameter as the payload position.
- Loaded the candidate passwords wordlist.
- Analyzed server responses to identify valid credentials.

### 4. Successful Authentication
Used the identified credentials to log in and access the account page.

## Key Learning Outcomes
- Username enumeration
- Authentication vulnerabilities
- Burp Suite Intruder
- HTTP response analysis
- Password brute-force testing

## Security Recommendations
- Use generic login error messages.
- Implement rate limiting.
- Enable multi-factor authentication (MFA).
- Monitor suspicious authentication attempts.

## Disclaimer
This lab was performed in the authorized PortSwigger Web Security Academy environment for educational purposes only.

**Lab Result: Successfully Solved**
