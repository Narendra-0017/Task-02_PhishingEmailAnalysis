# Task 2: Phishing Email Analysis

## Overview
This task involves analyzing a suspicious email and identifying phishing indicators based on sender information, header clues, language patterns, URLs, and attachments.

---

## 📩 Sample Email Analyzed

**Subject:** Your Account Will Be Suspended – Immediate Action Required  
**From:** support@paypaI-security.com  

Dear Customer,

We noticed unusual activity on your PayPal account. To avoid suspension,
you must verify your information immediately.

Click the link below to continue:
https://paypaI-security.com/verify/login

Failure to do so will result in permanent account restriction.

Thank you,
PayPal Support Team

**Attachment:** Account_Verification.html

---

## 🔍 Phishing Indicators Identified

### 1. Suspicious Sender Address
- The domain **paypaI-security.com** is fake.
- Uses capital “I” in place of lowercase “l” → classic spoofing trick.

### 2. Urgent / Threatening Language
- “Your account will be suspended”
- “Immediate action required”
- This is a common psychological pressure tactic.

### 3. Fake Verification Link
- URL: `https://paypaI-security.com/verify/login`
- Not a legitimate PayPal domain.
- Likely leads to a credential-harvesting site.

### 4. Generic Greeting
- “Dear Customer” — legitimate PayPal emails use the user's real name.

### 5. Suspicious Attachment
- HTML file named *Account_Verification.html*.
- Such files are usually phishing/credential-stealing forms.

### 6. Grammar & Formatting Issues
- Inconsistent capitalization.
- Unprofessional tone — typical in scam emails.

### 7. Header Red Flags (Conceptual)
If analyzed with a header analyzer:
- “Reply-To” mismatch  
- IP not belonging to PayPal  
- SPF/DKIM/DMARC failures  

---

## 🧰 Tools Used
- MXToolbox Header Analyzer  
- Manual link inspection  
- Standard phishing detection checklist  

---

## ✅ Conclusion
The email is clearly a phishing attempt designed to steal PayPal login credentials using domain spoofing, urgency, fake links, and deceptive attachments.

---

## 📁 Repository Contents
- `README.md` (this report)  
- `phishing_email_sample.txt` (raw email text)  
