# Jenkins #1

>>>>NEWSLIDE
## The story continues
![Image of Story](../res/img/stick_men_illustration.png)

>>>>NEWSLIDE
## Contents

* Build automation: _What is CI?_
* Hello, Jenkins World!
* CI: Fetching and building code

>>>>NEWSECTION

## Why bother?

* *"It works on my machine"*
* Environment differences
* Repetitive, manual work


>>>>NEWSLIDE
> "Our highest priority is to satisfy the customer
through early and continuous delivery
of valuable software."

## Why use a continuous integration server?
<img src="img/jenkinslogo.png" alt="Jenkinsbot" width="30%"/>



>>>>NEWSLIDE

> " Working software is the primary measure of progress. "

## Do my changes work:

  * On someone else's machine?
  * With everyone else's changes?
  * On all platforms?


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

 * Ensure our software is working
 * Increase our development efficiency
 * Work in teams
 * Single source of truth
 * Shorten the feedback loop

Not bad, eh?

> "Our time is always more valuable than machines' time"

>>>>NEWSECTION

##  Let's have a chat about the difference between CI and CoDe...
>>>>NEWSLIDE

![Image of Jenkinsbot](../../../shared/img/code-story.bare.png)

Note:  Let's talk about the difference between CI and CoDe

>>>>NEWSLIDE

##  We have options!

<img src="img/automation_platforms.jpg" alt="Platforms" width=60% />

>>>>NEWSLIDE

## But today we choose jenkins!
<img src="img/jenkinsbotwithlogo.jpeg" alt="Platforms" width=60% />


>>>>NEWSECTION
# Hello, Jenkins World!

>>>>NEWSLIDE
## Terminology
* Job
* Build
* Master / nodes
* Schedule
* Pipeline
* Plugins
* Jenkinsfile (Build_as_code)

>>>>NEWSLIDE
## Terminology explained

The Jenkins *master* is an advanced *scheduler* that on basis of *Job definitions* monitor and executes *builds* on *nodes*.
A *job* can be defined in many ways, as *Standard job*, through *JobDSL* or through the new *Jenkins Pipeline*.

>>>>NEWSLIDE
## Workflow of standard jobs
![Image of old pipelines](img/old.pipeline.png)


>>>>NEWSLIDE
## Pipelines
![Image of multibranch pipeline](img/a.multibranch.pipeline.png)

>>>>NEWSLIDE
![Image of Jenkinsbot](img/jenkinsbot.jpeg)


>>>>NEWSLIDE
## Architecture
![Image of Jenkinsbot](img/Jenkins-architecture-basic.png)


>>>>NEWSLIDE
## Architecture - Detailed
![Image of Jenkinsbot](img/Jenkins-architecture.png)

>>>>NEWSECTION
## Inside Jenkins

>>>>NEWSLIDE
## Jenkins UI

![Jenkins UI](img/jenkins.welcome.decorated.png)


>>>>NEWSLIDE

## Let's get to work!
Installing Jenkins on Ubuntu 16.04

https://www.digitalocean.com/community/tutorials/how-to-install-jenkins-on-ubuntu-16-04

###!NB No need for Step 3 - Opening the Firewall    
>>>>NEWSLIDE

## Let's see what happened!

    # Go check <HOST_IP>:8080
    # Create a job
    # What happened?



>>>>NEWSLIDE
# OK, now it's your turn!

    # Go check <HOST_IP>:8080
    # Create a job
    # What happened?

>>>>NEWSECTION
# Jenkins setup

>>>>NEWSLIDE
## Credentials
```
ubuntu@codeacgbg:~$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/home/ubuntu/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /home/ubuntu/.ssh/id_rsa.
Your public key has been saved in /home/ubuntu/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:uuO6VOGaQ9uIfhchgkpPz0PCGNAIo1OiM49jnvTfFq4 ubuntu@codeacgbg
```

>>>>NEWSLIDE
## Add credentials to Jenkins
```
ubuntu@codeacgbg:~$ cat /home/ubuntu/.ssh/id_rsa
-----BEGIN RSA PRIVATE KEY-----
MIIEpAIBAAKCAQEAwM1h3G70DCXaV85w30h2E8w1JKEFU46vf+vY562RU0tyzUXi
pj53ojajcMfkrxlq+DaoR0KC+i0dotrNVVROCsZI9mFQ0Yc6/7+nIZB6a4oGkONs
UuGIlY9dJ7Oo5j3FGUMp3/HpORZgF+2Qqq/GkYSTxW8kp01UUAWbY5csAaQyfn81
....
dZ4drQKBgQDz4Ywu9i2M8mFAOIbTAizCouPihZd66xHfESVO4mb1ny36xRwyth4M
Swnw8MsrlFJWZ/GAMyFRKDXrQTSJk6ygk/xCFhnCP28RvLF3Eqo79lxCTkJ3lk5B
niQ311mJ4wTCFtzYV5IEbwsbDt4OVpf1tytrXLwCCrOI8eMtnzTl3w==
-----END RSA PRIVATE KEY-----
```
>>>>NEWSLIDE
![Adding credentials to Jenkins](img/jenkins.add.credentials.png)

>>>>NEWSLIDE
## adding credentials to GitHub
```
ubuntu@codeacgbg:~$ cat .ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDAzWHcbvQMJdpXznDfSHYTzDUkoQVTjq9/69jnrZFTS3LNReKmPneiNqNwx+SvGWr4NqhHQoL6LR2i2s1VVE4Kxkj2YVDRhzr/v6chkHprigaQ42xS4YiVj10ns6jmPcUZQynf8ek5FmAX7ZCqr8aRhJPFbySnTVRQBZtjlywBpDJ+fzX0CciYY21qqqaKRdDrbf6zdQpPJvHaAGNFTeJihVhVJzeRrCoSsRw+bvm1xPFpE1RC8UGRKvziVfpXLCswZiqhrdbnyOS4dBBcOjVsfphwuvhVDq0XtaNCbC7WqTJdpQLXB9ZQzPRkclN+Wsk1RZTsrbFjGF845jzxlyM9 ubuntu@codeacgbg
```
>>>>NEWSLIDE
## adding credentials to GitHub
![credentials](img/github.credentials.png)

>>>>NEWSECTION
# Continuous Integration

## Is my code good enough to share with my team?

>>>>NEWSLIDE
## Let's "build" roman Gilded Rose
>>>>NEWSLIDE

## go fork the repo
![](img/github.fork.png)


>>>>NEWSLIDE

## CI is:

* Fetch
* Integrate
* Run tests

Not doing CI just yet, only building for today.

>>>>NEWSLIDE
## A Job is an atomic unit of automation work
<img src="img/jenkins.job.png" alt="Platforms" width=80% />

>>>>NEWSLIDE
### Now it's your turn
* Work on exercises 0 to *4.5 implementing the Gilded Rose*
https://github.com/praqma-training/gildedrose/blob/master/README.md
