# Web Recon & Misconfiguration Case Study

## 🧠 Overview
This project is a security research case study analyzing DNS misconfiguration and origin server exposure in a real-world web architecture.

It demonstrates how improper CDN configuration can expose backend infrastructure.

---

## 🎯 Objective
To understand:
- DNS behavior differences (apex vs www)
- CDN protection mechanisms
- Origin server exposure risks

---

## 🛠️ Tools Used
- dig (DNS enumeration)
- curl (HTTP analysis)
- httpx (service probing)

---

## 🔍 Key Finding
A misconfiguration was observed where:
- Subdomain traffic was routed through CDN
- Root domain pointed directly to origin IP

This creates a potential security bypass of CDN protection layer.

---

## 📄 Full Report
See: `case-study/report.md`

---

## ⚠️ Impact
- Exposure of origin server IP
- Bypass of CDN/WAF protection
- Increased attack surface

---

## 📚 Disclaimer
This project is for educational purposes only. No unauthorized testing was performed.
