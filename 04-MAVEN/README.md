# 04 – Maven

**Phase:** 🏗️ Build

## 📘 What is Maven?
Build and dependency management tool for Java projects using `pom.xml`.

## 🛡️ Why it matters in DevSecOps
Maven pulls third-party libraries – the main source of supply-chain vulnerabilities. Knowing the build lets you plug in SCA and SAST scans.

## 🔑 Key Concepts
- `pom.xml`, groupId / artifactId / version
- Lifecycle: validate → compile → test → package → verify → install → deploy
- Local (`~/.m2`) vs remote repositories
- Plugins (SonarQube, Dependency-Check)

## 💻 Important Commands / Example
```bash
mvn clean package
mvn test
mvn dependency:tree
mvn verify sonar:sonar
```

## ❓ Interview Questions
1. Explain the Maven lifecycle.
2. What is a transitive dependency?
3. How do you find which library brings a vulnerable dependency?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
