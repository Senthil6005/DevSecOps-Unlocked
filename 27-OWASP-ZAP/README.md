# 27 – OWASP ZAP

**Phase:** 🌐 DAST

## 📘 What is OWASP ZAP?
Open-source web application security scanner that attacks a running app to find vulnerabilities.

## 🛡️ Why it matters in DevSecOps
SAST reads code; ZAP tests the live app like a hacker would – finding issues such as XSS and missing security headers.

## 🔑 Key Concepts
- Baseline scan (passive) vs Full scan (active)
- Spider / crawler
- Alerts by risk level
- API scanning

## 💻 Important Commands / Example
```bash
docker run -t ghcr.io/zaproxy/zaproxy:stable zap-baseline.py -t https://your-app-url
docker run -t ghcr.io/zaproxy/zaproxy:stable zap-full-scan.py -t https://your-app-url
```

## ❓ Interview Questions
1. What is DAST?
2. SAST vs DAST?
3. Passive vs active scan?
4. Why only scan apps you own or are authorized to test?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
