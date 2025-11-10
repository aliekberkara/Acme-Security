## 📋 Submission Information

**Name:** Ali Ekber KARA  
**Email:** [aliekber123kara@gmail.com]  
**LinkedIn:** [linkedin.com/in/ali-ekber-kara] _(optional)_  
**Submission Date:** [YYYY-MM-DD]

---

## ✅ Deliverables Checklist

Please confirm you've included all required items:

- [+] **Report** (PDF, max 5 pages)
  - [+] Section 1: Incident Analysis
  - [+] Section 2: Architecture Review
  - [+] Section 3: Response & Remediation
  
- [+] **Video Presentation** (10-15 minutes)
  - [+] Link provided in `video.md`
  - [+] Video is accessible (tested in incognito)
  - [+] Duration is within guidelines

- [+] **File Structure**
```
  submissions/ali-ekber-kara/
  ├── Ali_Ekber_KARA_Report.pdf
  └── video.md
```

---

## 📊 Self-Assessment

**Time spent on this lab:** Approximately 12 hours

**Tools used:**
- Log analysis: VS Code
- Diagrams: Canva, Claude.ai
- Video recording: OBS Studio

**Confidence level:**
- [ ] Very confident in my analysis
- [+] Confident but some uncertainties
- [ ] Attempted my best with available knowledge

---

## 🎯 Brief Summary (2-3 sentences)

_Briefly describe your approach and key findings:_

[During the investigation, I correlated WAF, API, email, and web logs to reconstruct the attack chain.
The incident started with an IDOR vulnerability, followed by a phishing campaign, and ended with SQL Injection and data exfiltration.
My analysis identified the root causes and proposed a new defense-in-depth architecture to strengthen security.]

---

## 🔍 Key Findings Highlight

**Main attack vectors identified:**
1. IDOR (Insecure Direct Object Reference) in /api/v1/portfolio
2. Phishing campaign via fake domain acme-finance.com
3. SQL Injection in /dashboard/search

**Most critical vulnerability:**
Broken Access Control (IDOR) allowing attacker to enumerate user data

**Top recommendation:**
Implement MFA, enforce API-level ownership validation, and upgrade WAF rules to detect advanced injection attempts.

---

## 💭 Challenges & Learnings

**What was most challenging?**
The most challenging part was writing the incident report in a professional format. It required not only analyzing different log sources but also correlating them chronologically to find the root cause. Explaining complex security events such as IDOR, phishing, and SQL injection clearly and logically was difficult. Writing in a formal, evidence-based style also took extra time and attention.

**What did you learn?**
I learned how to connect technical findings with business impact and how to explain a cyber incident in a structured and professional way. I also improved my understanding of MITRE ATT&CK mapping, OWASP classifications, and the importance of log correlation for real-world investigations.

**What would you do differently?**
Next time, I would start with a clear incident map before writing the report. I would also automate part of the log normalization process to save time and focus more on analysis rather than formatting.

---

## 📝 Additional Notes _(optional)_

Any context, assumptions, or additional information you'd like evaluators to know:

The attacker used an IP range reserved for penetration testing (203.0.113.0/24), making detection more difficult.

SOC 2 Type II audit preparation influenced the security improvement recommendations.

All findings were validated with timestamp and log references.

---

## ⚖️ Declaration

I declare that:
- [+] This work is entirely my own
- [+] I have not copied from other submissions or answer keys
- [+] I have not modified the provided log files
- [+] All sources and tools are properly attributed
- [+] I understand plagiarism results in disqualification

**Signature:** Ali Ekber KARA  
**Date:** 2025-11-09

---

## 🚀 Ready for Review

By submitting this PR, I confirm that my work is complete and ready for evaluation.

---

_Thank you for your submission! Our team will review it within 1 week._