# Jockey Reusable Workflows

This repo contains several Github Actions Workflows, that are intended to be re-used across multiple different projects.

# DO NOT PUT PRIVATE INFORMATION IN THIS REPO

Due to Github limitations, this repo **must** be public, meaning exposed to the public internet.

---
# Code Checks

## nextjs-code-checks.yml
Performs `yarn install` for the current repo, with optional scripts that happen:

- Pre `yarn install`
- Post `yarn install`
- Post `yarn check-typescript && yarn check-eslint`

# Building & Deploying

## docker-build-with-args.yml
With the given information, it will run a `Dockerfile` in the root of the current repo, and then push the code up to the configured Container Registry

## docker-deploy-to-azure-app.yml
Given a Docker Container fully qualified name, it will deploy that image to the configured Azure App Service
