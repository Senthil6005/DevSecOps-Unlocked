# 21 – Kubernetes

**Phase:** ☸️ Orchestration

## 📘 What is Kubernetes?
Container orchestration platform that deploys, scales and manages containers across a cluster.

## 🛡️ Why it matters in DevSecOps
Kubernetes is the target of most deployments – and a misconfigured cluster can expose everything.

## 🔑 Key Concepts
- Pod, Deployment, Service, Namespace
- RBAC (Role, RoleBinding, ServiceAccount)
- Network Policies
- Secrets (base64 is NOT encryption)
- Pod Security Standards / securityContext

## 💻 Important Commands / Example
```bash
kubectl get pods -A
kubectl apply -f deploy.yaml
kubectl auth can-i delete pods --as dev-user
kubectl get networkpolicy -A
```

## ❓ Interview Questions
1. How do you secure a Kubernetes cluster?
2. What is RBAC?
3. Are Kubernetes Secrets encrypted?
4. What is a Network Policy?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
