# 26 – HashiCorp Vault

**Phase:** 🔐 Secrets Management

## 📘 What is HashiCorp Vault?
Tool to securely store, access and rotate secrets, tokens, certificates and encryption keys.

## 🛡️ Why it matters in DevSecOps
Removes hardcoded passwords from code and config; issues short-lived dynamic credentials.

## 🔑 Key Concepts
- Secrets engines (KV, AWS, database)
- Auth methods (token, Kubernetes, AppRole)
- Policies
- Dynamic secrets & leases
- Seal / unseal

## 💻 Important Commands / Example
```bash
vault server -dev
export VAULT_ADDR=http://127.0.0.1:8200
vault kv put secret/app db_pass=Secret123
vault kv get secret/app
```

## ❓ Interview Questions
1. Why use Vault instead of environment variables?
2. What are dynamic secrets?
3. Vault vs AWS Secrets Manager?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
