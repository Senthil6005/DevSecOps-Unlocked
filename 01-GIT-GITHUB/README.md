# 01 – Git & GitHub

**Phase:** 🧑‍💻 Code

## 📘 What is Git & GitHub?
Git is a distributed version control system; GitHub hosts Git repositories online with collaboration features.

## 🛡️ Why it matters in DevSecOps
Every secure pipeline starts from code. Branch protection, signed commits and pull-request reviews stop unreviewed or malicious code from reaching production.

## 🔑 Key Concepts
- Repository, commit, branch, merge, pull request
- Branch protection rules & required reviews
- Signed commits (GPG/SSH)
- `.gitignore` to keep secrets & build files out
- CODEOWNERS file

## 💻 Important Commands / Example
```bash
git init
git clone <url>
git checkout -b feature-login
git add . && git commit -m "msg"
git push origin feature-login
git log --oneline
git config --global commit.gpgsign true
```

## ❓ Interview Questions
1. Difference between git merge and git rebase?
2. What are branch protection rules?
3. How do you remove a secret that was already committed?
4. What is a signed commit?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
