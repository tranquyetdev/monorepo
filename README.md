# Apps

## NextJS

```bash
# Install the NextJS plugin
nx add @nx/next

# Create a new NextJS app
nx g @nx/next:app nextjs

# Install Nx Container plugin
nx add @nx-tools/nx-container
nx add @nx-tools/container-metadata

# Generate Dockerfile
nx g @nx-tools/nx-container:init --project=nextjs

# Make sure docker is running
# Invoke the container build target for an app
nx container nextjs

# Check the docker image
docker image ls

# Run the container image
docker run -p 3000:3000 nextjs:main
```
