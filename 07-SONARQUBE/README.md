# 07 – SonarQube

**Phase:** 🔍 SAST

## 📘 What is SonarQube?
Platform for continuous code quality and security inspection (bugs, vulnerabilities, code smells, security hotspots).

## 🛡️ Why it matters in DevSecOps
SonarQube is the most widely used SAST tool in enterprise pipelines; its Quality Gate blocks insecure code from merging.

## 🔑 Key Concepts
- Bugs, Vulnerabilities, Code Smells, Security Hotspots
- Quality Profiles & Quality Gates
- Coverage & duplication
- Integration with Jenkins/GitHub Actions

## 💻 Important Commands / Example
```bash
docker run -d --name sonarqube -p 9000:9000 sonarqube:lts-community
mvn sonar:sonar -Dsonar.host.url=http://<ip>:9000 -Dsonar.token=<token>
```

## ❓ Interview Questions
1. What is SAST?
2. Difference between a vulnerability and a security hotspot?
3. What is a Quality Gate?
4. Limitations of SAST?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
