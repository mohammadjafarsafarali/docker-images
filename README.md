# Get Images

A place for sharing Docker images to ditch the Docker Hub

## Where is the shared images?

All the shared Docker images are available here:

[https://github.com/users/dimagehub/packages](https://github.com/users/dimagehub/packages)

## How to publish a new image?

```
# Command:
docker tag {LOCAL-IMAGE-ID} ghcr.io/dimagehub/{IMAGE-NAME}:{IMAGE-TAG}
docker push ghcr.io/dimagehub/{IMAGE-NAME}:{IMAGE-TAG}

# Example:
docker tag cc8775c0fe94 ghcr.io/dimagehub/nginx:1.23.1-alpine
docker push ghcr.io/dimagehub/nginx:1.23.1-alpine
```

## How to use the shared images?

```
docker pull ghcr.io/dimagehub/nginx:1.19.3-alpine
OR
FROM ghcr.io/dimagehub/nginx:1.19.3-alpine
```
