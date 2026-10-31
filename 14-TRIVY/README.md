# 14 – Trivy

**Phase:** 🐳 Container & IaC Scanning

## 📘 What is Trivy?
All-in-one open-source scanner from Aqua Security for images, filesystems, Git repos, IaC and Kubernetes.

## 🛡️ Why it matters in DevSecOps
Trivy is the most popular container scanner – fast, free and easy to add to any pipeline.

## 🔑 Key Concepts
- Scan targets: image, fs, repo, config, k8s
- Severity filtering
- `--exit-code 1` to fail pipelines
- SBOM generation
- `.trivyignore` for accepted risks

## 💻 Important Commands / Example
```bash
trivy image nginx:latest
trivy image --severity HIGH,CRITICAL --exit-code 1 myapp:1.0
trivy fs .
trivy config ./terraform
trivy k8s --report summary cluster
```

## ❓ Interview Questions
1. How do you fail a build only on critical CVEs?
2. Trivy vs Snyk Container?
3. How do you reduce vulnerabilities in an image?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
