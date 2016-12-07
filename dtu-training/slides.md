# DST4L
## Collaborating through GitHub
Jan Krag & Thierry Lacour

>>>>NEWSECTION
## Who are we?
### Jan Krag
<img src="img/jan.png" alt="Jan Krag" width="30%"/>


Continuous Improvement Agent

Note:
* We work for Praqma, a consultancy company focusing on helping customers implement CoDe
* We'll not go into that now, Lars will show up to talk about that later
                  
>>>>NEWSECTION
## Who are we?
### Thierry Lacour
<img src="img/thierry.png" alt="Thierry Lacour" width="30%"/>


Automation Toolsmith

Note:
* Software developer
* Jack of all trades
* Backline support for people at customers 

>>>>NEWSECTION
## Who are you?
### Librarians
<img src="img/librarian.jpg" alt="The Librarian" width="30%"/>


Not our typical audience!

Note:
* We usually train software developers
* The training topic is also very "devy"
* Interested to see:
  * Your reaction
  * Your ideas
* If you're confused about the picture, it's from "The Librarian" movies, which I like more than I should.

>>>>NEWSECTION
## Roadmap
* Introduction to GitHub
* The GitHub Flow
* A local GitHub
* GitHub Pages

>>>>NEWSECTION
# Introduction to GitHub

>>>>NEWSECTION
## Quick intro
What is ...

Git?


GitHub?


A repository?

Note:
* Git is technology used to version files.
  * Git manages versions and allows for easy comparison/rollback/etc.
* GitHub is a collaboration platform built around Git
  * Big community, very popular, lots of successful open source projects
* The repository is the entity around which collaboration happens
  * It's the file store for a single project or component, etc.
  * Work, discussions and file changes happen in the scope of a repository

>>>>NEWSECTION
## Exploring a repository
Visit [github.com/Praqma/praqma.com](https://github.com/Praqma/praqma.com)

Note:
* Visit the [praqma.com](https://github.com/Praqma/praqma.com) repo
* `Code` 
  * repository bulk, where you keep all your files and data
* `README.md` 
  * 'Markdown' file rendered on the main page by default
  * Make sure you hand out MD cheat sheets 
* `Issues` 
  * The heart of collaboration & communication, where you manage work/report problems, etc.
* `Projects` 
  * A means to organize/plan your issues 
* `Pull Request` 
  * Pull requests are for proposing changes to the repo, owners can merge them in
* `Wiki` 
  * A place to hold documentation for your repo
* `Pulse` and `Graphs` 
  * Dashboards and useful data of your project
* `Settings` 
  * You don't see this unless you're an owner or admin  

>>>>NEWSECTION
## Team up!

* 3-4 members
* a team name
* a team captain

Note:
* Team captain announces their team name

>>>>NEWSECTION
## Setup
* Log in to [github.com](github.com)
* Visit [github.com/praqma-training/dst4l](github.com/praqma-training/dst4l)
* Head over to **Issues**
* Comment on the issue thread!
                           
Note:
* Now that you're teamed up, let's do some setup.
* Head over to the training repo and comment an the issue there.
* Anyone can create issues and comment on existing ones.
* But you have to be a collaborator to make any changes to the repository.
* Comment on the issue and we'll add you as a collaborator.
* **SETUP:** Add everyone as collaborators
 
>>>>NEWSECTION
## You've got mail!

Now is a good time to talk about:
* Thread subscription
* Repository watching

Note:
* Now that you've all gotten a bunch of emails, let's talk about controlling notifications
* GitHub sends you notifications of:
  * Issue threads you're subscribed to
  * Repositories you're watching
  * By default, you watch repositories you join (changed in profile settings)
* You can unsubscribe from issue threads
* You can unwatch repositories
* **DEMO:** Unwatch and unsubscribe from thread/repositories
* **DEMO:** Change notification settings in GitHub profile

>>>>NEWSECTION
## Our first commit

Create a new file in the repository:


**`team-name/member-name-bio.md`**

Tell us a bit about yourself!

Note:
* Explain that `foo/bar.md` creates a `bar.md` file in a `foo` directory
* Feel free to use Markdown to spice up your bio!
  * **Make sure the cheat sheets are handed out.**
* Write a nice message when committing the file to the repository!
* **When they're done:**
  * Go to the commit graph
  * Explain commits
    * Creates a safe rollback point for us.
    * Allows us to see our repo at a specific point in time.
    * Even allows us to rollback specific commits 

>>>>NEWSECTION 
## A quick recap

Git(Hub)


Repositories


Collaborators


Issues


Notifications

       
    
Note:
* GitHub is a collaboration platform around Git
* Git is a versioning control system used for managing file versions
* Repositories are the heart of a project, they hold the files and are the scope of issues
* Issues are discussion threads for problems/tasks to work on
* Notifications are eager to give you updates on issues, but don't get flooded by them!

>>>>NEWSECTION
# The GitHub Flow
                                    
>>>>NEWSECTION
## Setup

**Captains**


Create a team repository

**Members**


Go to your team repository
 
Note:
So let's create a repository
 * Create a repository yourself
 * Include a README file, handwave it for now
 * Have team captain create a repo

>>>>NEWSECTION
## Setup

**Members**


Create an issue: 

`"Add me as a collaborator!"`

**Captains**
* Add your members as collaborators
* Resolve their issue

Note:
* Issues are what drives work
* They describe problems, tasks, etc.
* Anyone can create issues on any repository
* Collaborators can make changes, branches and merge in PR's
* **DEMO:** (Jan) creates an issue to add Jan as collaborator
* Create an issue for your team captain add you as collaborator
* **DEMO:** Add Jan as collaborator to your demo repo. Resolve the issue   
* Team captain, add them in the settings page and resolve the issues!   

>>>>NEWSECTION 
## Go with the flow

## **[The GitHub Flow](https://guides.github.com/introduction/flow/)**

Note:
* Before we start working, let us propose a nice workflow
* Workflow promoted by GitHub themselves
* Let's take a quick peek
* **DEMO:** Go through GH Flow
* It focuses on tying your work to issues and promotes discussion of the changes you're making
* Let's do some work following this flow

>>>>NEWSECTION                                                                                                                                                      
## Propose a change!

* Choose an animal _(may be extinct)_
* Create an issue
  * `"Add my-animal"`
* Assign yourself

Note:
* Again, issues drive work, so let's get started.
* Pick any animal and create an issue to add that animal to your repository
* Assign yourself to the issue
* **DEMO:** Create an issue:
  * Title: Add sheep 
  * Content: 
    

Add sheep to our catalogue of critters:
    

 - [] Create a branch
    

 - [] Add a file with ASCII art
    

 - [] Commit the file
    

 - [] Open a PR
    

 - [] Discuss changes
    

 - [] Tweak changes
    

 - [] Merge PR
  * Demonstrate markdown for headers, checkboxes, etc.
    * Toolbar
    * `Preview`
  * Assign the issue to a yourself
  * Add a label  

>>>>NEWSECTION                                                                                                                                                      
## Branch off!

Create a branch:


`my-animal`

Note:                               
* Now we have our issue, let's do some work
* If you work on a branch, your work is isolated and doesn't bother others
* So let's make a branch to do some work
* Briefly discuss "Git Status" toolbar (commits, branches, releases, contributors) 
* **DEMO:** Creating a Branch          
* Create a branch named `thierry-bio`
* Demo what happens when you refresh the page/click on the main repo!
    
>>>>NEWSECTION                                                                                                                                                      
## Do some work!

Create a file for your animal


**`zoo/sheep.txt`**
```
                           .@@@.    "Baaaaahd art."
              .@#@#@#@#@/@/@/@@@     /
            .#@#@#@#@#@#@#@/@'u\   /
          *(|@#@#@#@#@#@#@#@(   \
              @#@#@#@#@#@#@# \ww/
               @#@#@#@#@#@# 
               ) //   | ||
               \ \\   | ||
                \ \\  | \\
                 """   """
```
**!!** Make sure you are on _your_ branch **!!**

Note:
* While we're on our branch, let's create a file
* **DEMO:** Create a file in a folder in the repository
  * `zoo/sheep.md`
  * Commit the file

>>>>NEWSECTION
## Open a pull request!

**Everyone**

* Head over to `branches`
* Open a pull request for your branch
* Reference your issue in the comment
  
Note:
* Now we've done our work, let's share it by opening a pull request
* Pull requests are a great tool for discussing changes and eventually merging them in
* **DEMO:** Creating a Pull Request on GitHub
  * Show `base:` and `compare:` drop downs
  * Reference issue from before "Hey, I did some work on #2"
  * Assign to captain, label as enhancement
  * Create PR  
* Return to original issue and hover over information pane                            

>>>>NEWSECTION
## Collaborate!
 
* Visit eachother's Pull Requests
* Collaborate:
  * Discuss improvements
  * Post ~~mean~~ *nice* comments
  * Tag with emoji's

Note:
* Let's take a look at this PR
* **DEMO**
 * `Conversation` view
 * `Commits` view
 * `Files changed` view
 * Create line comment
   * Add a general comment to the discussion
   * Add :+1: emoji

>>>>NEWSECTION
## Improve!

* Revisit your branch and file
* Improve it using the feedback you received

Note:
* After a healthy discussion on your issue, make some changes!
* **DEMO:** Edit the file based on the pull request comments
  * Show the `Commits` tab
  * Update the issue to discuss your new changes
  * Comment on other people's PR's: Good to go!

>>>>NEWSECTION
## Merge it in!

* Head back to your PR
* Merge in the pull request
* Mention your issue in the comment
  * `"This adds a sheep. Resolves issue #3."`
* Go find your issue

Note:
* So now our changes look really nice
* Let's merge them in!
* When you merge a pull request, the changes you've made get applied to the 'master' branch
  * Rule: Only merge your own pull request. Add :ship: to someone else's PR as example.
* **DEMO:** Merge the pull request, closing the issue in the merge commit
  * Discuss merge dropdown. Squash/Merge vs. default merge.
    * A squash merge 'squashes' your changes into a single commit
      * This deletes the commit history. 
  * IF: Merge attempt failed. 
    * Every time someone merges, GitHub checks for conflicts. 
    * If it doesn't have time to make the checks because of the amount of merges, it'll give us a 'Merge Attempt Failed' dialog. 
  * When it's done, deletes the branch
  * Show the closed issue                                                                            

>>>>NEWSECTION                                                                           
## A quick recap

* Open an issue
* Branch off
* Do some work
* Collaborate
* Merge

Note:
* Go over [the GitHub Flow](https://guides.github.com/introduction/flow/)** again

    NEWSECTION
### Resources

 - [https://services.github.com/classnotes/](https://services.github.com/classnotes/)    
 - [guides.github.com/features/mastering-markdown/](http://guides.github.com/features/mastering-markdown/)