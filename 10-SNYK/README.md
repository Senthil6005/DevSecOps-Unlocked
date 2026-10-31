# 10 – Snyk

**Phase:** 🔍 SCA & Developer Security

## 📘 What is Snyk?
Developer-first security platform that scans dependencies, containers, IaC and code, and suggests fixes.

## 🛡️ Why it matters in DevSecOps
Snyk shows the fix (upgrade version or patch), not just the problem – making developers fix issues faster.

## 🔑 Key Concepts
- Snyk Open Source, Container, IaC, Code
- Fix pull requests
- Monitoring for new CVEs
- Free tier for individuals

## 💻 Important Commands / Example
```bash
npm install -g snyk
snyk auth
snyk test
snyk container test myapp:latest
snyk iac test
```

## ❓ Interview Questions
1. Dependency-Check vs Snyk?
2. What is a fix PR?
3. How does continuous monitoring help after deployment?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
