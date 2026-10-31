# 28 – Argo CD

**Phase:** 🚀 GitOps

## 📘 What is Argo CD?
Declarative GitOps continuous delivery tool for Kubernetes.

## 🛡️ Why it matters in DevSecOps
Git becomes the single source of truth: every change is reviewed and auditable, and drift is automatically corrected.

## 🔑 Key Concepts
- GitOps principles
- Application, Project, Sync, Health
- Auto-sync & self-heal
- RBAC & SSO

## 💻 Important Commands / Example
```bash
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
argocd app list
argocd app sync myapp
```

## ❓ Interview Questions
1. What is GitOps?
2. Push vs pull deployment model?
3. How does Argo CD improve security?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
