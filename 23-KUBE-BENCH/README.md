# 23 – kube-bench

**Phase:** ☸️ Kubernetes Compliance

## 📘 What is kube-bench?
Aqua Security tool that checks a Kubernetes cluster against the CIS Kubernetes Benchmark.

## 🛡️ Why it matters in DevSecOps
Shows exactly which cluster settings are insecure, with remediation steps – required for compliance audits.

## 🔑 Key Concepts
- CIS Benchmark
- Checks for control plane, nodes, policies
- PASS / FAIL / WARN results
- Runs as a Kubernetes Job

## 💻 Important Commands / Example
```bash
kubectl apply -f https://raw.githubusercontent.com/aquasecurity/kube-bench/main/job.yaml
kubectl logs job/kube-bench
```

## ❓ Interview Questions
1. What is a CIS benchmark?
2. What can kube-bench check on a managed cluster like EKS?
3. How do you remediate failed checks?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
