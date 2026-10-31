# 13 – Hadolint

**Phase:** 🐳 Container – Dockerfile Linting

## 📘 What is Hadolint?
Linter that checks Dockerfiles for best practices and security mistakes.

## 🛡️ Why it matters in DevSecOps
Catches problems like `latest` tags, root user and unpinned packages before the image is even built.

## 🔑 Key Concepts
- Rules like DL3007 (avoid latest tag)
- Integrated ShellCheck for RUN commands
- Ignore rules via config
- Runs in CI and IDEs

## 💻 Important Commands / Example
```bash
docker run --rm -i hadolint/hadolint < Dockerfile
hadolint Dockerfile
```

## ❓ Interview Questions
1. Why lint a Dockerfile?
2. Name three Dockerfile best practices.
3. Why is the `latest` tag risky?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
