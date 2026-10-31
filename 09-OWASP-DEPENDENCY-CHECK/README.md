# 09 – OWASP Dependency-Check

**Phase:** 🔍 SCA

## 📘 What is OWASP Dependency-Check?
Free OWASP tool that identifies known vulnerabilities (CVEs) in project dependencies.

## 🛡️ Why it matters in DevSecOps
Most application code is open-source libraries. One vulnerable library (like Log4j) can compromise the entire app.

## 🔑 Key Concepts
- Software Composition Analysis (SCA)
- CPE matching against the NVD database
- HTML/XML/JSON reports
- Fail build on CVSS threshold

## 💻 Important Commands / Example
```bash
dependency-check.sh --project myapp --scan . --format HTML
mvn org.owasp:dependency-check-maven:check -DfailBuildOnCVSS=7
```

## ❓ Interview Questions
1. What is SCA?
2. What is NVD?
3. What happened with Log4Shell?
4. How do you fix a vulnerable transitive dependency?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
