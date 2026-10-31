# 03 – pre-commit Hooks

**Phase:** 🧑‍💻 Code – Shift-Left

## 📘 What is pre-commit Hooks?
A framework that runs checks automatically before every `git commit` on the developer's machine.

## 🛡️ Why it matters in DevSecOps
The most 'left' you can shift security: issues are blocked on the laptop before they ever reach the repository.

## 🔑 Key Concepts
- Git hooks (`.git/hooks/pre-commit`)
- `.pre-commit-config.yaml`
- Hooks for Gitleaks, linting, formatting, Terraform
- Same hooks can run in CI

## 💻 Important Commands / Example
```bash
pip install pre-commit
pre-commit install
pre-commit run --all-files
pre-commit autoupdate
```

## ❓ Interview Questions
1. What is a Git hook?
2. Difference between pre-commit and pre-push hooks?
3. Can developers bypass pre-commit? How do you enforce it?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
