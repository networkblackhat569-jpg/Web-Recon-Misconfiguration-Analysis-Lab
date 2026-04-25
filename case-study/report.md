# Security Misconfiguration Case Study

## 🎯 Summary
This research analyzes a misconfiguration where the origin server was directly accessible, bypassing CDN protection provided by :contentReference[oaicite:0]{index=0}.

---

## 🔍 Discovery Method
- DNS enumeration using `dig`
- HTTP probing using `curl` and `httpx`
- Direct IP access testing

---

## 🧪 Key Finding
- `www.domain.com` → Protected via CDN
- Root domain → Points directly to origin IP

This creates a bypass of CDN security layer.

---

## ⚠️ Impact Analysis

### Potential Risks:
- Direct origin exposure
- Bypass of WAF protections
- Increased attack surface
- Possible DDoS targeting origin IP

---

## 🧠 Technical Root Cause
- Incomplete CDN configuration
- Missing full proxy mode for apex domain
- Origin IP exposed in DNS records

---

## 🛠️ Recommendation
- Enable full proxy (CDN) for all DNS records
- Restrict origin server to CDN IP ranges only
- Block direct IP access via firewall
