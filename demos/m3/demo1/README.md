# Demo 1

Clean code - refactoring pipelines.

## 1.1 A real build pipeline

Log into Jenkins at http://localhost:8080 with `jenkins`/`jenkins`.

- New item, pipeline, `demo1-1`
- Select pipeline from source control
- Git - https://github.com/MijailStell/JenkinsForDocker.git
- Path to Jenkinsfile  - `demos/m3/demo1/1.1/Jenkinsfile`
- Open in Blue Ocean
- Run

> Walk through the [Jenkinsfile](./1.1/Jenkinsfile)

## 1.2 Adding parameters for RC build

- Copy item, `demo1-2` from `demo1-1`
- Path to Jenkinsfile `demos/m3/demo1/1.2/Jenkinsfile`
- Open in Blue Ocean
- Run (first build doesn't show option)

> Walk through the [Jenkinsfile](./1.2/Jenkinsfile)

- Run again - _RC = no_
- Run again - _RC = yes_

> Check logs and artifacts

## 1.3 Moving pipeline logic into Groovy methods

- Copy item, `demo1-3` from `demo1-1`
- Path to Jenkinsfile `demos/m3/demo1/1.3/Jenkinsfile`
- Build now
- Run

> Walk through the [Jenkinsfile](./1.3/Jenkinsfile)

- Open in Blue Ocean
- Run again - _RC = no_
- Run again - _RC = yes_

> Check logs and artifacts