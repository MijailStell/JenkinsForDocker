# Module 4

Powering pipelines with Docker.
Shared pipelines and the Job DSL plugin.
Using multi-branch pipelines.

## Pre-reqs

Run Jenkins in [Docker](https://www.docker.com/products/docker-desktop):

```
docker-compose -f jenkins/docker-compose.yml up -d
```

> Plugins configured in [install-plugins.groovy](jenkins/clean/scripts/install-plugins.groovy)

## 4 Create Folder

Log into Jenkins at http://localhost:8080 with `jenkins`/`jenkins`.
- New item, fodler, `m4`
- All demos will be done **inside** this folder
