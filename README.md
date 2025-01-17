This repository demonstrates a common mistake in Dockerfiles: using the `latest` tag for the base image.  The `latest` tag can change unexpectedly, breaking builds and introducing security vulnerabilities.  This example shows how to fix the issue by specifying a specific, stable version.

**Problem:**
The original `Dockerfile` uses `ubuntu:latest`. This is insecure and unreliable for production deployments.

**Solution:**
The fixed `Dockerfile` uses a specific version of Ubuntu (e.g., `22.04`). This ensures consistent and reproducible builds and reduces security risks.