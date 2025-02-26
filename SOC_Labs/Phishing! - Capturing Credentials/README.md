# Phishing Lab - Capturing Credentials 🎣

## Overview
This lab demonstrates how attackers use **phishing techniques** to steal user credentials. We will use the **Social Engineering Toolkit (SET)** to create a fake login page and capture credentials.

⚠️ **For educational purposes only! Do not use this for illegal activities.**  

## Lab Contents
- **01_Getting_Started/** → Lab setup and environment information
- **02_Go_Phish/** → Phishing attack using SET
- **03_Lab_Complete/** → Wrap-up and lessons learned
- **screenshots/** → Demo images and results

## 1️⃣ Attacker Setup
### Steps to Create a Phishing Page

1. **Open the Linux Console** (This represents the attacker's machine).
2. **Start the Social Engineering Toolkit (SET)**:
   ```sh
   sudo setoolkit
   ```
   > If the command fails, wait a few minutes and try again (files might still be installing).

3. **Accept the Terms of Service**: Type `y` and press **Enter**.
4. **Select Social-Engineering Attack**:
   ```
   1) Social-Engineering Attacks
   
5. **Select Website Attack Vectors**:
   ```
   2) Website Attack Vectors

6. **Select Credential Harvester Attack Method**:
   ```
   3) Credential Harvester Attack Method
   ```
7. **Choose Web Templates Method**:
   ```
   1) Web Templates
   ```
8. **Enter the IP address for the POST request** (Default: `172.31.24.5`). Press **Enter**.
9. **Select Google Login Page Template**:
   ```
   2) Google Template
   ```

**At this point, SET is creating a fake Google login page that will capture any credentials entered.**

---

## 2️⃣ Victim Simulation
### Steps to Simulate the Victim
1. **Switch to the Windows Desktop** (simulating the victim’s machine).
2. **Open Firefox Browser**.
3. **Enter the attacker’s IP in the address bar**:
   ```
   172.31.24.5
   ```
4. **Observe the Google Login Page** (images may not load in the lab environment).
5. **Enter test credentials**:
   ```
   Email: susieq@company.com
   Password: topsecretpassword
   ```
6. **Click Sign In**.
   
---

## 3️⃣ Lab Analysis - Viewing Captured Credentials
1. **Switch back to the Linux Desktop (attacker’s machine).**
2. **Check for captured credentials**:
   ```sh
   cat /var/www/html/logs.txt
   ```
3. **Observe how phishing attacks capture user credentials.**

---

## Key Takeaways 🛡️
- **Phishing is a common attack method**: Attackers use fake websites to steal credentials.
- **Be cautious of email links**: Always verify the URL before entering login details.
- **Use Multi-Factor Authentication (MFA)**: This adds an extra layer of security.
- **Report phishing attempts**: If you receive a suspicious email, report it to your security team.

### How to Defend Against Phishing Attacks
✅ Verify URLs before entering login credentials.  
✅ Be skeptical of urgent or unexpected login requests.  
✅ Never reuse passwords across multiple sites.  
✅ Enable Multi-Factor Authentication (MFA).  
✅ Report suspicious emails to your IT security team.  

---

## Contributing 🤝
If you'd like to contribute to this repository, feel free to submit pull requests with improvements or additional scenarios!

📌 **Educational Use Only!** Do not use this knowledge for malicious purposes.
