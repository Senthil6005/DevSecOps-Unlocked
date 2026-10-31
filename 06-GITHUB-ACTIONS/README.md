# 06 – GitHub Actions

**Phase:** 🏗️ CI/CD

## 📘 What is GitHub Actions?
CI/CD service built into GitHub; workflows are written in YAML under `.github/workflows/`.

## 🛡️ Why it matters in DevSecOps
Security scans run on every push and pull request. Actions also support OIDC to access AWS without long-lived keys.

## 🔑 Key Concepts
- Workflow, job, step, runner
- Triggers: push, pull_request, schedule
- GitHub Secrets & environments
- OIDC authentication to AWS
- Pinning actions to a commit SHA (supply-chain safety)

## 💻 Important Commands / Example
```yaml
name: security-scan
on: [push, pull_request]
jobs:
  scan:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: echo "run scans here"
```

## ❓ Interview Questions
1. Jenkins vs GitHub Actions?
2. What is OIDC and why is it safer than access keys?
3. Why pin third-party actions to a SHA?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
