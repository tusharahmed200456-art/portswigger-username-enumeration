Username Enumeration via Response Timing

Lab Information

Platform: PortSwigger Web Security Academy

Difficulty: Practitioner

Category: Authentication

Tool: Burp Suite Professional

Status: solved

1. What I Learned

In this lab, I learned how a website can reveal valid usernames through response time.

Sometimes a website shows the same error message for every login attempt. However, the server may take different amounts of time to process different usernames.

This difference can help identify a valid username.

2. Tools I Used

Burp Suite Professional

Burp Proxy

Burp Repeater

Burp Intruder

3. My Testing Process

Step 1: Intercept Login Request

I opened the login page and entered test credentials.

Then I captured the login request using Burp Suite Proxy.

Step 2: Analyze the Response

I checked the HTTP response and observed the login error message.

The website displayed a similar error message for incorrect login attempts.

Step 3: Response Time Analysis

I learned that response time can provide useful information about how the server processes usernames.

I compared multiple login requests to understand the timing differences.

Step 4: Username Testing

I used the provided candidate username list to test usernames in the authorized lab environment.

Step 5: Password Testing

After identifying a valid username, I tested the provided candidate password list to find the correct password.

Step 6: Account Access

The final objective is to log in successfully and access the account page.

4. What I Learned from This Lab

What username enumeration means.

How response timing works.

How to use Burp Repeater.

How to configure Burp Intruder.

How authentication systems process login requests.

Why timing differences can create security risks.

5. Security Recommendations

Use generic login error messages.

Make login processing time consistent.

Implement rate limiting.

Monitor suspicious login attempts.

Enable Multi-Factor Authentication.

Disclaimer

This testing was performed in the authorized PortSwigger Web Security Academy lab environment for educational purposes.

My Learning Note

This lab helped me understand that a website can reveal information not only through error messages but also through response timing.
