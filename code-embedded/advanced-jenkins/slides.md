# Jenkins Pipelines
![](img/jenkinslogo.png)<!-- .element height="30%" width="30%" -->

>>>>NEWSLIDE
## Introducing Pipelines
No more pointy pointy, cliky cliky

![](img/pointclick.jpeg)

>>>>NEWSLIDE
## Motivations for pipelines as code

* Retain history of all changes to Pipeline
* Rollback to a previous Pipeline version
* View diffs and merge changes to the Pipeline
* Test new Pipeline steps in branches
* Run the same Pipeline on a different Jenkins server


>>>>NEWSLIDE
## Jenkins Pipeline
[Jenkins Pipeline](https://jenkins.io/doc/book/pipeline/) is a suite of plugins which supports implementing and integrating continuous delivery pipelines in Jenkins.


>>>>NEWSLIDE
## Two Syntax Options

* Scripted Pipelines
  * Original
  * Flexibility and extensibility
  * Steep learning curve
* Declarative:
  * Simpler and more opinionated
  * Stricter structure
  * Requires less groovy knowledge

**Today we will use declarative syntax**

>>>>NEWSLIDE
## UI
Showing the stages of the pipeline
![](img/pipeline.png)

>>>>NEWSLIDE
## Scripted Jenkinsfile

```
node {
    stage('Build') {
        sh 'make'
    }
}
```


>>>>NEWSLIDE
# Vocabulary

* Stage
* Node
* Step

>>>>NEWSLIDE
## Scripted Jenkinsfile
Several nodes
```
node('linux') {
    stage('Build') {
        sh 'make'
    }
}
node('linux&&ubuntu') {
    stage('Test') {
        sh 'make check'
        junit 'reports/**/*.xml'
    }
}
node('linux&&deployment'){
    stage('Deploy') {
        sh 'make publish'
    }
}
```

>>>>NEWSLIDE
Two job-types for pipelines

- Pipeline

![](img/job.pipeline.png)

- Multi-branch Pipeline

![](img/job.multibranch.pipeline.png)

>>>>NEWSECTION
# Your first pipeline

>>>>NEWSLIDE
Create a new job in Jenkins.

Give it a good name and select the 'pipeline' type

[Getting Started](https://jenkins.io/doc/book/pipeline/getting-started/) provides nice help for those new to this.
![](img/new-item-creation.png)

>>>>NEWSLIDE
## Making your first pipeline
Do exercise **5,6,7** in the [Embedded Project repository](https://github.com/praqma-training/embeddedproject).


>>>>NEWSECTION
## Additional methods:
- Archiving

```
// archiving the jar files in the target folder
archiveArtifacts 'target/*.jar'

```


>>>>NEWSLIDE
## Additional methods:
- Docker

```
node{
withDockerContainer('ubuntu:latest') {
    sh 'echo "hello world"'
}}

```

or

```
node{
sh 'docker run -i --rm --name my-maven-project -v "$PWD":/usr/src/mymaven -w /usr/src/mymaven maven:3-jdk-8 mvn -Dmaven.test.failure.ignore clean package'
}
```

>>>>NEWSLIDE

##Exercises 7+8

* [7](https://github.com/praqma-training/gildedrose#7-archiving)
* [8](https://github.com/praqma-training/gildedrose#8-dockerize-this)


>>>>NEWSECTION
## Multibranch pipeline

Creates a set of Pipeline projects according to detected branches in one SCM repository.

So every branch on your remote becomes a pipeline. Just push and it will be triggered!


>>>>NEWSLIDE

##Exercises 9

* [9](https://github.com/praqma-training/gildedrose#9-multibranch-pipeline)

>>>>NEWSECTION
## Advanced methods
- Parallel

```
// Define
def builders = [
	"build": {
		node {}
	},
	"javadoc": {
	node {}
	}
]
stage('parallel'){
	parallel builders
}

```

- Stash/unstash
```
// archiving the jar files in the target folder
archiveArtifacts 'target/*.jar'

```

>>>>NEWSECTION
# Pretested integration flow

>>>>NEWSLIDE

The end goal:
- Our _master_ branch is _pristine_
- No bad code goes to master!

>>>>NEWSLIDE

The plan:
- Write-protect the master branch
- Have developers flag when they have code they want _integrated_
- Have Jenkins listen for branches to integrate
- Jenkins decides ( through tests ) whether or not the code can go to master

>>>>NEWSLIDE

The tools:
- Pretested Integration Plugin
- Listen for branches named `ready/**`
- Integrate into master branch

>>>>NEWSLIDE
![CoDe:U Branching Strategy](img/code-u-branching.png)
<!--- TODO Take Thierrys Git Phlow drawing instead of this --!>

>>>>NEWSLIDE
![PIP Configuration](img/pip-config.png)

>>>>NEWSLIDE
![PIP Configuration cont.](img/pip-config2.png)
