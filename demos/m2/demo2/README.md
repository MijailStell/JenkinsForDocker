# Demo 2

Modelling workflows in pipelines

## 2.1 A multi-stage pipeline

Go to http://localhost:8080/job/m2/

- New item, pipeline, `demo2-1`
- Select pipeline from source control
- Git - https://github.com/MijailStell/JenkinsForDocker.git
- Branch: main
- Path to Jenkinsfile `demos/m2/demo2/2.1/Jenkinsfile`

> Walk through the [Jenkinsfile](./2.1/Jenkinsfile)

- Run and check 
- **Fails** because step in second stage uses unknown variable

## 2.2 Requesting user input

Back to http://localhost:8080/job/m2/

- Copy item, `demo2-2` from `demo2-1`
- Path to Jenkinsfile `demos/m2/demo2/2.2/Jenkinsfile`

> Walk through the [Jenkinsfile](./2.2/Jenkinsfile)

- Run and check
- Pauses on input stage - OK or abort
- Post runs every time

## 2.3 Parallel stages

Back to http://localhost:8080/job/m2/

- Copy item, `demo2-3` from `demo2-1`
- Path to Jenkinsfile `demos/m2/demo2/2.3/Jenkinsfile`

> Walk through the [Jenkinsfile](./2.3/Jenkinsfile)

- Run and check
- Parallel stages complete in any order
- Then pause on input and then post
