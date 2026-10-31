# 16 – Cosign (Sigstore)

**Phase:** 🐳 Supply Chain – Image Signing

## 📘 What is Cosign (Sigstore)?
Tool to sign and verify container images so only trusted images are deployed.

## 🛡️ Why it matters in DevSecOps
Signing proves an image came from your pipeline and was not tampered with – protecting the Integrity in the CIA triad.

## 🔑 Key Concepts
- Key-pair signing vs keyless (OIDC) signing
- Signatures stored in the registry
- Verify before deploy (with Kyverno)
- Attestations (SBOM, provenance)

## 💻 Important Commands / Example
```bash
cosign generate-key-pair
cosign sign --key cosign.key <user>/myapp:1.0
cosign verify --key cosign.pub <user>/myapp:1.0
```

## ❓ Interview Questions
1. Why sign container images?
2. What is keyless signing?
3. How do you enforce only signed images in Kubernetes?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
