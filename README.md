# Phishing-Analysis-tools-Phishing-Case-1

![image](https://github.com/user-attachments/assets/6f8a8a7f-66ff-446e-acdd-0df85a8d106e)

## Phishing Case 1: Analyzing Suspicious Emails

### Scenario:

As a Level 1 SOC Analyst, I was tasked with investigating several suspicious emails forwarded to me by coworkers. My responsibility was to analyze these emails to extract critical details, which would then be used by my team to implement rules to prevent future spam/phishing emails from reaching our colleagues.
Task:

Using the tools and resources discussed, I was to analyze each email's header and body to answer specific questions about the nature and origin of these emails.
Analysis and Findings

#### 1. What brand was this email tailored to impersonate?

![image](https://github.com/user-attachments/assets/d23c0735-57c4-4888-a74e-895151e07206)

    Answer: Netflix
    
Explanation: I utilized PhishTool to analyze the content of the email. The tool provided information that indicated the email was designed to impersonate Netflix. This was evident from the visual elements, language, and overall formatting that mimicked Netflix's branding.

#### 2. What is the From email address?

![image](https://github.com/user-attachments/assets/fbcbc7db-447b-4186-a3c1-c51b141583af)

    Answer: JGQ47wazXe1xYVBrkeDg-JOg7ODDQwWdR@JOg7ODDQwWdR-yVkCaBkTNp.gogolecloud.com

Explanation: By examining the email header, I identified the "From" email address. The address was obfuscated, likely as a tactic to evade detection by automated filters, but it could be extracted directly from the header information.

#### 3. What is the originating IP? Defang the IP address.

![image](https://github.com/user-attachments/assets/6a2cf232-24ba-4612-80b4-7b6458012048)

    Answer: 209[.]85[.]167[.]226

    ![image](https://github.com/user-attachments/assets/5b4aa3cf-aa93-493c-90b2-a29e1bd08772)

Explanation: I used CyberChef, a versatile tool for analyzing and transforming data, to defang the IP address found in the email header. This process involved replacing the periods in the IP address with "[.]" to prevent accidental clicks or visits to a potentially malicious site.

#### 4. From what you can gather, what do you think will be a domain of interest? Defang the domain.

![image](https://github.com/user-attachments/assets/8b1e1815-fb0c-4d62-8d96-da02930b2891)

    Answer: etekno[.]xyz
    
Explanation: The domain of interest was identified from the "Return-Path" field in the email header. I again used CyberChef to defang the domain by altering the periods to "[.]," ensuring it could be referenced safely without risk of visiting the malicious site.

#### 5. What is the shortened URL? Defang the URL.


![image](https://github.com/user-attachments/assets/93f589a7-b09c-47e7-bdce-ec072b4f0331)

    Answer: hxxps[://]t[.]co/yuxfzm8kpg?amp=1
    
Explanation: The shortened URL was extracted from the message body, where it was presented as a clickable link. I defanged the URL using CyberChef to prevent any accidental navigation to the potentially harmful site by replacing "https" with "hxxps" and periods with "[.]."


#### Tool Proficiency: 

This project significantly improved my proficiency with tools like PhishTool and CyberChef. I gained hands-on experience in extracting and analyzing email headers and defanging URLs and IP addresses.
    
#### Analytical Skills: 

#### Experience Gained:

I enhanced my ability to dissect and interpret email components, which is crucial for identifying phishing attempts and other social engineering tactics.
Security Awareness: The project deepened my understanding of how phishing campaigns are constructed and the importance of scrutinizing every element of an email.

### Benefits

#### Enhanced Detection Capabilities: 

The experience gained from this project will enable me to better detect and analyze phishing attempts, thereby contributing to the overall security posture of my organization.
    
#### Improved Incident Response: 

By understanding the nuances of phishing emails, I can more effectively respond to incidents and prevent future attacks, thereby reducing the risk of data breaches or compromised accounts.

### Conclusion

This phishing analysis project provided valuable insights into the tactics used by cybercriminals to deceive users. By carefully analyzing email headers, bodies, and URLs, I was able to identify critical information that would help in creating defensive measures against such attacks.

