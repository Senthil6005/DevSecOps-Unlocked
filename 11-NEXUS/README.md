# 11 – Nexus Repository

**Phase:** 🏗️ Artifact Management

## 📘 What is Nexus Repository?
Repository manager that stores build artifacts (JARs, Docker images, npm packages) in one trusted place.

## 🛡️ Why it matters in DevSecOps
Using a private trusted repository protects against dependency confusion and tampered public packages.

## 🔑 Key Concepts
- Hosted, Proxy and Group repositories
- Release vs Snapshot
- Access control & cleanup policies
- Integration with Maven `settings.xml`

## 💻 Important Commands / Example
```bash
docker run -d -p 8081:8081 --name nexus sonatype/nexus3
mvn deploy   # after configuring distributionManagement in pom.xml
```

## ❓ Interview Questions
1. Why use an artifact repository?
2. Hosted vs proxy repository?
3. What is a dependency confusion attack?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
