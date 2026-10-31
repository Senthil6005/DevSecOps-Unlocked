# 05 – Jenkins

**Phase:** 🏗️ CI/CD

## 📘 What is Jenkins?
Open-source automation server used to build, test, scan and deploy applications through pipelines.

## 🛡️ Why it matters in DevSecOps
Jenkins is the 'orchestrator' of DevSecOps – it runs every security scan as a pipeline stage and can fail the build on critical findings.

## 🔑 Key Concepts
- Declarative pipeline (`Jenkinsfile`)
- Agents / nodes
- Credentials management (never hardcode)
- Plugins: SonarQube, OWASP, Docker, Kubernetes
- Securing Jenkins itself: RBAC, CSRF, updates

## 💻 Important Commands / Example
```groovy
pipeline {
  agent any
  stages {
    stage('Build') { steps { sh 'mvn clean package' } }
    stage('SAST')  { steps { sh 'mvn sonar:sonar' } }
    stage('Scan Image') { steps { sh 'trivy image myapp:latest' } }
  }
}
```

## ❓ Interview Questions
1. Declarative vs scripted pipeline?
2. How do you store secrets in Jenkins?
3. How do you fail a pipeline on critical vulnerabilities?
4. How do you secure a Jenkins server?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
