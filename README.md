# PHISHING-EMAIL
PHISHING EMAIL ANALYZER

This repository demonstrates my hands-on phishing analysis skills acquired through Let'sDefend. Below is a step-by-step walkthrough of how I analyzed a phishing email and identified the associated malicious activity.

**Objective**: Investigate the email header to identify suspicious elements.
-
-![first pic](https://github.com/user-attachments/assets/b383adf1-a927-4011-bac7-0515ca165893)

- **Tools Used**: Email header parsers, Let'sDefend dashboard. VirusTotal.com
- **Key Findings**:
  - Source IP: 216.244.76.116
  - Domain: storage.googleapis.com
  - Suspicious Subject Line: `WIR HABEN SIE ANGERUFEN, SIE HABEN NICHT GEANTWORTET
 
  - ![return path with answer 2nd pic](https://github.com/user-attachments/assets/6aa125cf-1fcc-49b5-b709-3e9f40b24f86)


In this step I break down the email by viewing the source of the email and looking for the return path. By viewing this return path I am able to 
detect spoofing, Ensure email deliverability, supports authentication protocols and improves trust. Always treat the email as suspicious if the
return path is unrelated.

![Domain Name 3rd pic](https://github.com/user-attachments/assets/144f0246-c2e5-4ade-8f33-8ffb29fc8efb)

While digging through the email source I was able to find the domain name of URL in the email. This is an important find because this helps
assess the legitimacy and safety of the email. The reason for this is, Cybercriminals often use fake domains that resemble legitimate ones to 
trick users.
5 ways Finding the Domain Name of an email is important is
1. Identifies Potential Spoofing.
2. Verifies Sender Authenticity.
3. Detects Malicious Activity.
4. Supports Security Protocols.
5. Protects Users from Phishing Attacks.

![virus tool 4th pic](https://github.com/user-attachments/assets/6dfce76f-ab4a-4b26-8a8a-9d766194ca61)



This final step, I used VirusTotal as a tool to find the body SHA-256 of the domain. Finding the SHA-256 hash of an email URL ensures the 
content's integrity, as any changes will alter the hash. It allows for secure sharing of malicious URLs without exposing sensitive data. 
Security systems can quickly compare the hash against known threats, improving detection and response times.
