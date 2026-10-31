# 20 – AWS Security Services

**Phase:** ☁️ Cloud Security

## 📘 What is AWS Security Services?
AWS native services to secure accounts and workloads: IAM, KMS, Secrets Manager, GuardDuty, Security Hub, Inspector, CloudTrail, WAF.

## 🛡️ Why it matters in DevSecOps
Most production DevSecOps pipelines deploy to the cloud; securing the account itself is as important as securing the code.

## 🔑 Key Concepts
- Shared Responsibility Model
- IAM least privilege, roles over access keys, MFA
- KMS encryption
- GuardDuty (threat detection), Inspector (vulnerability scanning), Security Hub (central findings)
- CloudTrail (audit logs), WAF (web protection)

## 💻 Important Commands / Example
```bash
aws iam list-users
aws guardduty list-detectors
aws securityhub get-findings --max-items 5
aws cloudtrail lookup-events --max-results 5
```

## ❓ Interview Questions
1. Explain the Shared Responsibility Model.
2. IAM user vs IAM role?
3. GuardDuty vs Inspector vs Security Hub?
4. How do you detect who deleted a resource?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
