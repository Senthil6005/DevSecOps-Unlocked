# 19 – Ansible

**Phase:** 🏗️ Configuration Management & Hardening

## 📘 What is Ansible?
Agentless automation tool that configures servers using YAML playbooks over SSH.

## 🛡️ Why it matters in DevSecOps
Used to harden servers automatically (disable root login, patch, firewall) consistently across hundreds of machines.

## 🔑 Key Concepts
- Inventory, playbook, task, module, role
- Idempotency
- Ansible Vault for secrets
- CIS hardening roles

## 💻 Important Commands / Example
```bash
ansible all -m ping -i inventory
ansible-playbook -i inventory harden.yml
ansible-vault create secrets.yml
```

## ❓ Interview Questions
1. What is idempotency?
2. How do you store passwords in Ansible?
3. Ansible vs Terraform?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
