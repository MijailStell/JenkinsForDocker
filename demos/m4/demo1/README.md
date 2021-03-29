# Demo 1

Powering pipelines with Docker.

## 1.1 Using a container as a build agent

Log into Jenkins at http://localhost:8080 with `jenkins`/`jenkins`.

- New item, pipeline, `demo1-1`
- Select pipeline from source control
- Git - https://github.com/MijailStell/JenkinsForDocker.git
- Path to Jenkinsfile  - `demos/m4/demo1/1.1/Jenkinsfile`
- Run

> Walk through the [Jenkinsfile](./1.1/Jenkinsfile)

## 1.2 Custom container agents

- Copy item, `demo1-2` from `demo1-1`
- Path to Jenkinsfile `demos/m4/demo1/1.2/Jenkinsfile`
- Run - fails

> Walk through the [Dockerfile](../Dockerfile) and the [Jenkinsfile](./1.2/Jenkinsfile)

> Walk through the fixed [Dockerfile.sdk](../Dockerfile.sdk) and [Jenkinsfile.fixed](./1.2/Jenkinsfile.fixed)

- Change Jenkinsfile to `demos/m4/demo1/1.2/Jenkinsfile.fixed`
- Run again

## 1.3 The Docker pipeline plugin

- Credentials in Jenkins - Docker Hub

- Copy item, `demo1-3` from `demo1-1`
- Path to Jenkinsfile `demos/m4/demo1/1.3/Jenkinsfile`
- Run

> Walk through the [Jenkinsfile](./1.3/Jenkinsfile) and [Dockerfile](../Dockerfile)
