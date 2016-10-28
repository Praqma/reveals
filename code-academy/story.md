# Chapter 1: The use case

So, you're an awesome guy. You know your way around
code, and while studying you made a cool hobby project.

A local business noticed your cool project and offered you a bunch of money ( which is nice ) if only you can show them a __Proof of Concept__ running on their __Cloud__ .

## Task
Set the project up to run on AWS

## Purpose
To get all the students up and running with the toolchain and enable the technical parts of all the following courses. To get them started with the entire toolchain and introduced the project

# Chapter 2: The first feature request

Good news! Your customer is back, your proof of concept works and he wants to pay you to add another feature!
You were working on some bugfix now - but your customer wants the feature now?
What should you do, when can the customer expect his feature.

You realize that you need some way of managing your tasks.

## Task
Go through Lego Scrum Game

## Purpose
Teach Agile Task management

# Chapter 3: S#!¤, I broke it ?!?!

While working on the new feature you went down a rabbit hole - Now you have no idea how to get back - And your code doesn't work at the moment.

You probably should have soe sort of versioning system.

## Task
Start using Git with the project

## Purpose
Teach them basic Git

# Chapter 4: Feature, feature, feature, ...

The client is really happy with your product - they keep requesting
features.  You have to make multiple releases and deployments each
week. You are lucky and most of them actually succeed. Some fail
though - and the process is boring - you want to have the process
automated.

## Task
Set up a Jenkins pipeline to deploy the project

## Purpose
Teach them enough Jenkins to keep them going throughout the week

# Chapter 5: An old feature broke

You are now releasing automatically, and feel happy about your
process.  After a new feture release however, your biggest client
complains that one of the old, stable features broke.

You feel like you didn't touch this feature and are unsure what the cause of the failure was. How can you prevent this in the future?

## Task

Set up a test pipeline for your project.

## Purpose

Teach them about the purpose of testing, and different types of testing.

## Notes

We're thinking about handing them a ton of tests and then have them figure out what is functional testing, and set up the pipeline accordingly with the principles of fast feedback, and running the "cheap" tests first.

# Chapter 6: Scaling Development

Your customers are happy, so you've brought in a few of your buddies
to help.  While developing a feature, you put your code on the master
branch and now it doesn't build. It turns out something in the work
that you've done the last week is not compatible with the work of your
friend.  You start wondering what part of the code is broken, and if
you could've worked in a smarter way.

## Task
Set up Continuous Integration with Pretested Integration on the project

## Purpose
Teach them about the benefits of Continuous Integration, and make the project pipeline even more awesome!

# Chapter 7: Production Fails

You've released some code after testing it thoroughly, but after
deploying it to the customers environment, it didn't work.
How can you make sure that this does not happen.

## Task
Dockerize the project

## Purpose
Teaching about Docker, and the benefits of containerization and productino like environments

# Chapter 8: I already did that ... Didn't I?

The customer requested a feature last month and asks if it is
deployed.  You think it was released but you are not quite sure, and a
bit confused about when it would have been released, and what code
actually implemented the feature. How to get this knowledge

## Task
Set up waffle, GHI for the project

## Purpose
Teach traceability and how to tie commits to your pipeline.

## Notes
In due time this should probably teach tracey.