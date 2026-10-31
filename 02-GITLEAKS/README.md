# 02 – Gitleaks

**Phase:** 🧑‍💻 Code – Secrets Scanning

## 📘 What is Gitleaks?
Open-source tool that detects hardcoded secrets (passwords, API keys, tokens) in Git repos and files.

## 🛡️ Why it matters in DevSecOps
Leaked AWS keys or DB passwords in GitHub are one of the most common causes of breaches. Gitleaks finds them before they are pushed.

## 🔑 Key Concepts
- Secret detection using regex rules
- Scans full Git history, not just current files
- Custom rules via `.gitleaks.toml`
- Baseline / allowlist for false positives

## 💻 Important Commands / Example
```bash
gitleaks detect --source . -v
gitleaks detect --report-format json --report-path leaks.json
gitleaks protect --staged     # scan before commit
```

## ❓ Interview Questions
1. Why are hardcoded secrets dangerous?
2. What do you do if a secret is found in Git history?
3. How to integrate Gitleaks in CI/CD?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
