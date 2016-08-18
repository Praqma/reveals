## Contents

1. Hello, Jenkins World!
2. CI: Fetching and building code
3. Pretested Integration
4. CoDe: Testing and evaluating code
5. Everything as code

>>>>NEWSECTION
# Hello, Jenkins World!

>>>>NEWSLIDE
![Image of Jenkinsbot](img/jenkinsbot.jpeg)

>>>>NEWSLIDE

> "Our highest priority is to satisfy the customer
through early and continuous delivery
of valuable software."

## Why use a continuous integration server?
<img src="img/jenkinslogo.png" alt="Jenkinsbot" width="30%"/>



>>>>NEWSLIDE

> " Working software is the primary measure of progress. "

## Do my changes work:

  * on someone else's machine?
  * with everyone else's changes?
  * on all platforms?


>>>>NEWSLIDE

> "Deliver working software frequently, from a
couple of weeks to a couple of months, with a
preference to the shorter timescale."

## Does my software:

  * Build itself?
  * Test itself?
  * Deploy itself?

>>>>NEWSLIDE

> Simplicity--the art of maximizing the amount
of work not done--is essential.

## Is my team:

  * Automating repetitive manual work?
  * Discovering errors quickly?
  * Avoiding rework?

>>>>NEWSLIDE

## So, an automation platform helps us:

 * ensure our software is working
 * increase our development efficiency
 * work in teams

Not bad, eh?

>>>>NEWSLIDE

##  Let's have a chat about the difference between CI and CoDe...


>>>>NEWSLIDE

![Image of Jenkinsbot](img/STORYLINE_A1_v2.jpg)

Note:  Let's talk about the difference between CI and CoDe

>>>>NEWSLIDE

##  So for both CI and CoDe...we need an automation platform!

>>>>NEWSLIDE

##  We have options!

<img src="img/automation_platforms.jpg" alt="Platforms" width=60% />

>>>>NEWSLIDE

## But today we choose jenkins!
<img src="img/jenkinsbotwithlogo.jpeg" alt="Platforms" width=60% />

>>>>NEWSLIDE

## Let's get to work!

    docker run -p 8080:8080 -p 50000:50000 jenkins
    # Go check <HOST_IP>:8080
    # Create a job
    # Stop the container
    # Restart the container
    # What happened?

>>>>NEWSLIDE

## Let's try again :-)

    mkdir jenkins
    docker run --name myjenkins -p 8080:8080 -p 50000:50000 \
               -v $PWD/jenkins:/var/jenkins_home \
               jenkins
    # Go check <HOST_IP>:8080
    # Create a job
    # Stop the container
    # Restart the container
    # What happened?

>>>>NEWSLIDE

<img src="img/jenkins.welcome.png" alt="Platforms" width=80% />

>>>>NEWSLIDE
# OK, now it's your turn!

    mkdir jenkins
    docker run --name myjenkins -p 8080:8080 -p 50000:50000 \
               -v $PWD/jenkins:/var/jenkins_home \
               jenkins
    # Go check <HOST_IP>:8080
    # Create a job
    # Stop the container
    # Restart the container
    # What happened?

>>>>NEWSECTION
# Continuous Integration

## Is my code good enough to share with my team?

>>>>NEWSLIDE
## Let's "build" adventure time!
<img src="img/Original_Finn.png" alt="Platforms" width=20% />

>>>>NEWSLIDE

## CI is:

* Fetch
* Integrate
* Run tests

>>>>NEWSLIDE
## A Job is an atomic unit of automation work
<img src="img/jenkins.at.newjob.png" alt="Platforms" width=80% />

>>>>NEWSLIDE

<img src="img/jenkins.at.build.png" alt="Platforms" width=80% />

>>>>NEWSLIDE

<img src="img/jenkins.at.vcs.png" alt="Platforms" width=80% />

>>>>NEWSLIDE

<img src="img/jenkins.at.project.png" alt="Platforms" width=80% />

Note:
Here we want to show:

  * Build job
  * Workspac

>>>>NEWSLIDE

<img src="img/jenkins.at.console.png" alt="Platforms" width=80% />

>>>>NEWSLIDE
# Ok, let's actually do a test

>>>>NEWSLIDE

<img src="img/jenkins.at.buildstep.png" alt="Platforms" width=80% />
<img src="img/jenkins.at.console.pass.png" alt="Platforms" width=80% />

>>>>NEWSLIDE
# But can it fail?
## Now is the time to create your own fork...

>>>>NEWSLIDE

<img src="img/at.fork.png" alt="Platforms" width=80% />
<img src="img/at.forked.png" alt="Platforms" width=80% />

>>>>NEWSLIDE

<img src="img/at.edit.fail.png" alt="Platforms" width=80% />

>>>>NEWSLIDE

## Remember to update the job urls!
<img src="img/jenkins.at.update.url.png" alt="Platforms" width=80% />

>>>>NEWSLIDE

<img src="img/jenkins.at.build.fail.png" alt="Platforms" width=40% />
<img src="img/jenkins.at.build.fail.console.png" alt="Platforms" width=80% />

>>>>NEWSLIDE

## Task 1: make the build pass again
## Task 2: make the build run automatically

>>>>NEWSECTION

# Pre-tested Integration
<img src="img/pretested.integration.png" alt="Platforms" width=80% />

>>>>NEWSLIDE

### 1. Install plugin
### 2. Configure pre-tested integration
### 3. Push good change to deliver and see it merge
### 4. Push bad change to deliver and see it rejected

>>>>NEWSECTION

# CoDe: Testing and evaluating code

>>>>NEWSLIDE
### 1. Set up verification job
### 2. Set build job to trigger it
### 3. "Deploy" the artifact

>>>>NEWSECTION

# Everything as code

>>>>NEWSLIDE

### 1. Create jobDSL for jobs
### 2. Create seedjob
### 3. Remove manually created jobs
