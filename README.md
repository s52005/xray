# Xray Docker Image
Dockerized Xray image, automatically built and published to Docker Hub and GitHub Container Registry using GitHub Actions.
<br><br/>
## Using the image
```shell
docker run -d \
  --name xray \
  --restart unless-stopped \
  -v /path/to/config.json:/etc/xray/config.json:ro \
  -p 1080:1080 \ # Depends on the inbound configs inside config.json
  s52005/xray:latest
```
<br><br/>
✅ Use a specific version tag from the repository’s Tags menu, such as v26.3.27, instead of the latest tag. Pinning a version helps prevent unexpected changes and compatibility issues.
<br><br/>
Checkout the Dockerfile and GitHub Actions workflow on GitHub:

[GitHub Repository](https://github.com/s52005/xray)

**Latest version:** ![](https://img.shields.io/badge/V-26.3.27-blue)

