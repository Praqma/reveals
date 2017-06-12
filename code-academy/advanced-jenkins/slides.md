# Jenkins Pipelines

>>>>NEWSLIDE
[Jenkins Pipeline](https://jenkins.io/doc/book/pipeline/) is a suite of plugins which supports implementing and integrating continuous delivery pipelines into Jenkins.

>>>>NEWSLIDE
2 Approaches:

Declarative or Scripted

>>>>NEWSLIDE
Declarative Jenkinsfile
```
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'make'
            }
        }
        stage('Test'){
            steps {
                sh 'make check'
                junit 'reports/**/*.xml'
            }
        }
        stage('Deploy') {
            steps {
                sh 'make publish'
            }
        }
    }
}
```
>>>>NEWSLIDE
Scripted Jenkinsfile

```
node {
    stage('Build') {
        sh 'make'
    }

    stage('Test') {
        sh 'make check'
        junit 'reports/**/*.xml'
    }

    stage('Deploy') {
        sh 'make publish'
    }
}
```
>>>>NEWSLIDE
Two job-types for pipelines

- Pipeline
- Multi-branch Pipeline

>>>>NEWSECTION
# My first pipeline

>>>>NEWSLIDE
Create a new job in jenkins. Give it a good name and select the pipeline-type

[Getting Started](https://jenkins.io/doc/book/pipeline/getting-started/) provides nice help for those new to this.

[My First Pipeline](http://localhost:8080/view/Pipelines/job/FirstPipeline/)




>>>>NEWSECTION
# A better pipeline

>>>>NEWSLIDE
Create a new job in Jenkins where you select the Multi-branch pipeline-type.

[Jenkins.io](https://jenkins.io/doc/book/pipeline/multibranch/) have a nice description how to get going.

[A better pipeline](http://localhost:8080/view/Pipelines/job/BetterPipeline/)

>>>>NEWSECTION
## Automated git flow
- Problem: my master broke, so i need to wait for the guy to fix it.
- Solution: Protect master with a Jenkins Pipeline that only commits changes that build.

>>>>NEWSLIDE
##pretested integration setup
