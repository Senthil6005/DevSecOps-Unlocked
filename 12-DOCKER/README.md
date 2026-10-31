# 12 – Docker

**Phase:** 🐳 Containers

## 📘 What is Docker?
Platform to package applications and dependencies into lightweight, portable containers.

## 🛡️ Why it matters in DevSecOps
Containers are the deployment unit of modern apps. Insecure images (root user, old base images) are a major attack surface.

## 🔑 Key Concepts
- Image, container, Dockerfile, registry
- Multi-stage builds to reduce size
- Run as non-root user (`USER app`)
- Minimal base images (alpine, distroless)
- Never put secrets in images

## 💻 Important Commands / Example
```bash
docker build -t myapp:1.0 .
docker run -d -p 8080:8080 myapp:1.0
docker images ; docker ps
docker history myapp:1.0
docker push <user>/myapp:1.0
```

## ❓ Interview Questions
1. Image vs container?
2. How do you make a Docker image secure?
3. What is a multi-stage build?
4. Why avoid running containers as root?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
