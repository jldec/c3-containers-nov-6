# c3-containers-nov-6
Based on [containers template](https://github.com/cloudflare/templates/tree/main/containers-template)

This repo works on arm-based MacOS machines. wrangler will invoke the docker build with '--platform linux/amd64' and Docker Desktop will happily run the image using rosetta to emulate x86.

The go build in the Dockerfile detects the platform from the container and cross-compiles to target linux/amd64 automatically. No additional configuration is required in the Dockerfile.

#### To learn more
- [Container docs](https://developers.cloudflare.com/containers/)
- [Container class](https://github.com/cloudflare/containers)
