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
