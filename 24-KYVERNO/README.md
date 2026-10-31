# 24 – Kyverno

**Phase:** ☸️ Policy as Code

## 📘 What is Kyverno?
Kubernetes-native policy engine; policies are written as Kubernetes YAML.

## 🛡️ Why it matters in DevSecOps
Blocks insecure deployments automatically – e.g., privileged pods, `latest` tags or unsigned images.

## 🔑 Key Concepts
- Validate, Mutate, Generate, VerifyImages policies
- Admission controller
- Enforce vs Audit mode
- Policy reports

## 💻 Important Commands / Example
```bash
helm repo add kyverno https://kyverno.github.io/kyverno/
helm install kyverno kyverno/kyverno -n kyverno --create-namespace
kubectl get clusterpolicy
kubectl get policyreport -A
```

## ❓ Interview Questions
1. What is policy as code?
2. Kyverno vs OPA Gatekeeper?
3. What is an admission controller?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
