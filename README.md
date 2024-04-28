# Docker iperf3 server

Dockerfile to setup a simple iperf3 server based on Alpine

## Supported architectures

`x86-64` `arm64v8` `arm32v7`

## Multi-platform build

```bash
# Create a builder
docker buildx create --name multi-builder

# Set the builder
docker buildx use multi-builder

# Build and publish
docker buildx build --platform linux/amd64,linux/arm/v7,linux/arm64/v8 -t registry.domain.com/iperf3:latest --push .
```
