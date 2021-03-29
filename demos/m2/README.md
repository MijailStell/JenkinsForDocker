# Module 2

Modelling workflows in pipelines & Adding pipeline build functionality

## Pre-reqs

Run Jenkins in [Docker](https://www.docker.com/products/docker-desktop):

```
docker-compose -f jenkins/docker-compose.yml up -d
```

> Plugins configured in [install-plugins.groovy](jenkins/context/scripts/install-plugins.groovy)

## 2 Create Folder

Log into Jenkins at http://localhost:8080 with `jenkins`/`jenkins`.
- New item, fodler, `m2`
- All demos will be done **inside** this folder
