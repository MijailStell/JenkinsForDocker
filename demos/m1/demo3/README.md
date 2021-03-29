## 1.1 Create a simple pipeline

- Go to http://localhost:8080/job/m1
- New item, pipeline, `demo1-1`
- Select sample pipeline script
- Replace echo with `echo "This is build number $BUILD_NUMBER"`
- Run and check output

## 1.2 Create a pipeline with Blue Ocean

Browse to http://localhost:8080/blue

- New pipeline
- Git repo - https://github.com/MijailStell/CleanPipiline.git
- Log in with Git creds

> Needs write access to repo

- Build pipeline
- Add environment variable `DEMO=1`
- Add stage
- Add _Print message_ `This is build $BUILD_NUMBER of demo $DEMO`
- Run and check: doesn't interpolate strings
- View Jenkinsfile in repo:editor only uses single quotes
- Replace with shell script `echo "This is build $BUILD_NUMBER of demo $DEMO"`

## 1.3 Create a pipeline from Git

- Back in the classic UI http://localhost:8080/job/m1
- New item, pipeline, `demo1-3`
- Select pipeline from source control
- Git - https://github.com/MijailStell/JenkinsForDocker.git
- Branch: main
- Path to Jenkinsfile `demos/m1/demo3/1.3/Jenkinsfile`

> Walk through the [Jenkinsfile](./1.3/Jenkinsfile)

- Run and check 
- Open in blue ocean
- Repeat stage