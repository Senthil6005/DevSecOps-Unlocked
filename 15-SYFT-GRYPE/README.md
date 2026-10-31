# 15 – Syft & Grype

**Phase:** 🐳 Supply Chain – SBOM

## 📘 What is Syft & Grype?
Syft generates a Software Bill of Materials (SBOM); Grype scans an SBOM or image for vulnerabilities.

## 🛡️ Why it matters in DevSecOps
SBOMs are becoming mandatory in many industries – they show exactly what is inside your software.

## 🔑 Key Concepts
- SBOM formats: SPDX, CycloneDX
- Generate once, scan anytime
- Track components across releases

## 💻 Important Commands / Example
```bash
syft myapp:1.0 -o cyclonedx-json > sbom.json
grype sbom:sbom.json
grype myapp:1.0
```

## ❓ Interview Questions
1. What is an SBOM?
2. SPDX vs CycloneDX?
3. How does an SBOM help when a new CVE is announced?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
