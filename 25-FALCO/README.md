# 25 – Falco

**Phase:** ☸️ Runtime Security

## 📘 What is Falco?
CNCF runtime security tool that detects suspicious behaviour in containers and hosts using system calls.

## 🛡️ Why it matters in DevSecOps
Scanners find problems before deployment; Falco catches attacks happening live (e.g., shell opened inside a container).

## 🔑 Key Concepts
- Rules, conditions, macros, outputs
- eBPF-based event capture
- Alerts via Falcosidekick (Slack, etc.)

## 💻 Important Commands / Example
```bash
helm repo add falcosecurity https://falcosecurity.github.io/charts
helm install falco falcosecurity/falco -n falco --create-namespace
kubectl logs -n falco -l app.kubernetes.io/name=falco
```

## ❓ Interview Questions
1. What is runtime security?
2. Give examples of Falco detections.
3. Static scanning vs runtime detection?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
