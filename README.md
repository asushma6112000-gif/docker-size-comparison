Docker Image Optimization Hands-on Lab (Normal vs Multi-Stage vs Distroless)

This repository demonstrates a hands-on practice session to understand Docker image optimization using different build strategies:

- Normal Docker Image
- Multi-Stage Docker Image
- Distroless Docker Image

---

## Hands-on Objective

To practically learn how Docker image size and security change with different build approaches and understand real DevOps optimization techniques.

---

## Tech Stack

- Python
- Docker
- Multi-Stage Builds
- Distroless Images

---

## Hands-on Structure

```

docker-size-comparison/
│
├── app.py
├── requirements.txt
├── Dockerfile.normal
├── Dockerfile.multistage
├── Dockerfile.distroless
└── screenshots/

```id="r2"

---

## Image Size Comparison (Practical Output)

```

normal-python-app        415MB
multistage-python-app    47.1MB
distroless-python-app    24.1MB

```id="r3"

---

## Hands-on Evidence (Screenshots)

- docker-image-size-comparison.png  
- multi-stage-docker-build.png  
- distroless-docker-build.png  

---

## What I Learned (Step by Step)

### 1. Docker Basics (Hands-on)
- Understood how Docker builds images using Dockerfile instructions
- Each instruction creates a separate layer

### 2. Normal Image Behavior
- Built a full Python image
- Observed large image size (400MB–1GB+)
- Learned it contains unnecessary OS packages and cache

### 3. Multi-Stage Build Practice
- Created separate build and runtime stages
- Reduced image size significantly
- Only required files are copied into final image

### 4. Distroless Image Practice
- Used minimal runtime-only image
- No shell or package manager included
- Improved security and reduced size

### 5. Final Comparison Result
- Normal → Heavy image  
- Multi-stage → Optimized image  
- Distroless → Minimal and secure image  

---

## Key Hands-on Takeaways

- Docker image optimization is essential in real DevOps workflows  
- Multi-stage builds reduce unnecessary dependencies  
- Distroless images improve security and reduce attack surface  
- Smaller images improve deployment speed and efficiency  

---

## Conclusion

This hands-on lab helped me understand real-world Docker optimization techniques used in production environments to improve performance, security, and efficiency.

