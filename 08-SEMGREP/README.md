# 08 – Semgrep

**Phase:** 🔍 SAST

## 📘 What is Semgrep?
Fast, lightweight, open-source static analysis tool with rules written in a code-like syntax.

## 🛡️ Why it matters in DevSecOps
Developers love it because it is fast and rules are easy to write – perfect for pre-commit and PR checks.

## 🔑 Key Concepts
- Rulesets (e.g., `p/owasp-top-ten`)
- Custom rules in YAML
- Supports many languages
- SARIF output for GitHub code scanning

## 💻 Important Commands / Example
```bash
pip install semgrep
semgrep --config auto .
semgrep --config p/owasp-top-ten --sarif -o results.sarif .
```

## ❓ Interview Questions
1. SonarQube vs Semgrep?
2. How do you handle false positives?
3. What is SARIF?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
