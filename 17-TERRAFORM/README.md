# 17 – Terraform

**Phase:** 🏗️ Infrastructure as Code

## 📘 What is Terraform?
IaC tool by HashiCorp to create and manage cloud infrastructure using declarative `.tf` files.

## 🛡️ Why it matters in DevSecOps
Infrastructure created by code can be reviewed and scanned for misconfigurations before it is created.

## 🔑 Key Concepts
- Provider, resource, variable, output, module
- State file (contains sensitive data – store remotely & encrypted)
- Remote backend: S3 + DynamoDB/state locking
- plan before apply

## 💻 Important Commands / Example
```bash
terraform init
terraform fmt ; terraform validate
terraform plan
terraform apply
terraform destroy
```

## ❓ Interview Questions
1. What is Terraform state and why protect it?
2. How do you manage secrets in Terraform?
3. What is drift?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
