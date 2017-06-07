<!--

 To include this markdown in your reveal add the following section:

  <section data-markdown="name-of-your-markdown.md"
    data-separator="^>>>>NEWSECTION$"
    data-separator-vertical="^>>>>NEWSLIDE$"
    data-separator-notes="^Note:$">
  </section>

-->

# Phlow

>>>>NEWSLIDE

## Problems in software development


Keeping track of work coming in - and getting it done<br/><!-- .element class="fragment" -->

Too much friction in the systems<br/><!-- .element class="fragment" -->

Branching strategies<br/><!-- .element class="fragment" -->

Release strategies<br/><!-- .element class="fragment" -->

>>>>NEWSLIDE

## As a developer


**I want**<br> 
Features that support the process that makes development easier

Transparancy in contributions. What is delivered, what is in progress

**So that**<br> 
I don't have to go to many different tools, to organize and manage my work flow

I don't have to wait for manual processes

>>>>NEWSLIDE

## As a product owner

**I want**<br> every single commit to happen for a documented reason, and that reason should be tied to the the commit

**So that**<br> When I need an overview I can just browse the commit history


>>>>NEWSECTION
## Solution?

![CoDe factory floor](../shared/img/code-story.bare.png)<!-- .element: class="plain max" -->

<!-- .slide: data-transition="slide-in none" -->


>>>>NEWSLIDE

## What is the solution

Make it easy<br/><!-- .element class="fragment" -->

Tie tasks to commits<br/><!--  .element class="fragment"  -->

Release train<br/><!-- .element class="fragment" -->

Milestones and office hours<br/><!-- .element class="fragment" -->

Automate all the things<br/><!-- .element class="fragment" -->

Any CI (Jenkins, Travis, Concourse)<br/><!-- .element class="fragment" -->



>>>>NEWSECTION

# git phlow

<br>
- git extension
- Provides tracebility
- Access tasks from the commandline
- Three Command Workflow

>>>>NEWSLIDE
## How it works

- Removes complex git commands
- Creates branches as workspaces
- Pushing changes
- Uses GitHub's API

>>>>NEWSLIDE

### Installation

Installation and setup is easy

<div> <!-- .element class="fragment" -->
```shell 
brew tap praqma/praqma-tap
brew install git-phlow
git phlow auth
git phlow mkalias
``` 
</div> <!-- .element class="fragment" -->


>>>>NEWSLIDE
## How to use git phlow

```shell
ghi open -m "Some new issues - I'd like to work on"
git workon 1
git wrapup --hard
git deliver --local
```

<div><!-- .element class="fragment" -->
workon - wrapup -deliver - workon - wrapup - deliver - workon - wrapup - deliver
</div><!-- .element class="fragment" -->


>>>>NEWSECTION

## Demo

Outline (Issues, Repositories, Waffle)

Installation

Workon 

Wrapup

Deliver

>>>>NEWSECTION

## Roadmap

- Code Café
- Community
- Features
    - Jira support
    - Windows
    - Apt-get installer
- More CI support


>>>>NEWSECTION

## Questions?

>>>>NEWSECTION

# Pull Requests 

>>>>NEWSLIDE

## Problems

- Context switching
- Time never comes around
- Everyone is waiting for someone to review
- People just accepts

>>>>NEWSLIDE
## Alternatives

Pair programming

Collaboration requests