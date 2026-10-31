# 18 – Checkov

**Phase:** 🏗️ IaC Security Scanning

## 📘 What is Checkov?
Open-source static analysis tool by Prisma Cloud for Terraform, CloudFormation, Kubernetes, Dockerfile and Helm.

## 🛡️ Why it matters in DevSecOps
Finds misconfigurations like public S3 buckets, open security groups and unencrypted volumes before deployment.

## 🔑 Key Concepts
- Hundreds of built-in policies (CIS, best practices)
- Scan Terraform plan JSON
- Skip checks with inline comments
- Custom policies in Python/YAML

## 💻 Important Commands / Example
```bash
pip install checkov
checkov -d ./terraform
checkov -f main.tf --compact
checkov -d . --framework kubernetes
```

## ❓ Interview Questions
1. Name 3 common cloud misconfigurations.
2. Checkov vs Trivy config?
3. How do you suppress a check with justification?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
