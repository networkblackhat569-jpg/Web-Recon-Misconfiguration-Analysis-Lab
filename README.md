# Web Recon & Misconfiguration Analysis

## 🔍 Overview

This project demonstrates practical web reconnaissance and analysis of DNS, CDN behavior, and server misconfigurations using tools like dig, curl, httpx, and nmap.

The goal is to understand how modern web infrastructure works and how misconfigurations can expose origin servers.

---

## 🧪 What I Tested

- DNS resolution differences between apex and www domain
- HTTP response behavior (redirects, status codes)
- CDN protection behavior via :contentReference[oaicite:0]{index=0}
- Origin server accessibility via direct IP access
- Security filtering and blocking behavior

---

## 🛠️ Tools Used

- dig (DNS analysis)
- curl (HTTP requests)
- httpx (web probing)
- nmap (network scanning)

---

## 📊 Key Observations

- `www` domain routed through Cloudflare
- Root domain resolved to direct origin IP
- HTTP 301 redirect from HTTP to HTTPS
- Cloudflare blocked automated requests (403 responses)
- Origin server remained directly accessible via IP

---

## 📚 What I Learned

- Difference between CDN-protected and direct-hosted architecture
- DNS misconfigurations can expose origin servers
- Importance of restricting origin access to CDN IP ranges
- HTTP status codes in security analysis
- Real-world web infrastructure behavior

---

## ⚠️ Disclaimer

This project is for educational and ethical learning purposes only.
No unauthorized testing was performed.
