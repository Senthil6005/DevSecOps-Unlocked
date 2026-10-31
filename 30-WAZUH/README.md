# 30 – Wazuh

**Phase:** 📊 SIEM & XDR

## 📘 What is Wazuh?
Open-source security platform for threat detection, log analysis, file integrity monitoring and compliance.

## 🛡️ Why it matters in DevSecOps
Brings all security logs together (servers, cloud, containers) to detect and respond to incidents – the final layer of DevSecOps.

## 🔑 Key Concepts
- SIEM concepts
- Wazuh manager, indexer, dashboard, agents
- File Integrity Monitoring (FIM)
- Vulnerability detection & compliance (PCI DSS, CIS)

## 💻 Important Commands / Example
```bash
# Install agent (example – Ubuntu)
sudo systemctl status wazuh-agent
sudo systemctl restart wazuh-agent
```

## ❓ Interview Questions
1. What is a SIEM?
2. What is File Integrity Monitoring?
3. Logging vs monitoring vs SIEM?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
