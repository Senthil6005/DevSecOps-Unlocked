# 22 – Helm

**Phase:** ☸️ Kubernetes Packaging

## 📘 What is Helm?
Package manager for Kubernetes; charts bundle all manifests with configurable values.

## 🛡️ Why it matters in DevSecOps
Secure defaults can be built into charts once and reused by every team.

## 🔑 Key Concepts
- Chart, release, values.yaml, templates
- Repositories
- Upgrade & rollback
- Scan charts with Checkov/Trivy

## 💻 Important Commands / Example
```bash
helm create myapp
helm install myapp ./myapp
helm upgrade myapp ./myapp
helm rollback myapp 1
helm template ./myapp | checkov -f - 
```

## ❓ Interview Questions
1. What is a Helm chart?
2. How do you roll back a release?
3. How do you manage secrets with Helm?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
