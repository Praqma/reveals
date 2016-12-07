# DST4L
## Collaborating through GitHub
Jan Krag & Thierry Lacour

>>>>NEWSECTION
## Who are we?
### Jan Krag
<img src="img/jan.png" alt="Jan Krag" width="30%"/>
<br />Continuous Improvement Agent

Note:
Maybe some points you want to talk about
                  
>>>>NEWSECTION
## Who are we?
### Thierry Lacour
<img src="img/thierry.png" alt="Thierry Lacour" width="30%"/>
<br />Automation Toolsmith

Note:
* Software developer
* Jack of all trades
* Backline support for people at customers
* We work for Praqma, a consultancy company focusing on helping customers implement CoDe
* We'll not go into that now, Lars will show up to talk about that later 

>>>>NEWSECTION
## Who are you?
### Librarians
<img src="img/librarian.jpg" alt="The Librarian" width="30%"/>
<br />Not our typical audience!

Note:
* We usually train software developers
* The training topic is also very "devvy"
* Interested to see:
  * Your reaction
  * Your ideas

>>>>NEWSECTION
## Roadmap
* Hands-on intro to GitHub
* Powertalk by [@lakruzz](https://github.com/lakruzz)
* 


>>>>NEWSECTION
## Quick intro
What is ...

Git?
<br />GitHub?
<br />a repository?

Note:
* Git is technology used to version files.
  * Git manages versions and allows for easy comparison/rollback/etc.
* GitHub is a collaboration platform built around Git
  * Big community, very popular, lots of successful open source projects
* The repository is the entity around which collaboration happens
  * It's the file store for a single project or component, etc.
  * Work, discussions and file changes happen in the scope of a repository

>>>>NEWSECTION
## Setup
Make teams!
* 3-4 members
* a team leader
* a team name

Note:
* Team leads announce their team names
                                    
>>>>NEWSECTION
## Setup
Log in to [github.com](github.com) and...

**Leaders**
<br />Create a repository!

**Members**
<br />Go to your lead's repository
 
Note:
So let's create a repository
 * Create a repository yourself
 * Include a README file, handwave it for now
 * Have team leads create a repo

>>>>NEWSECTION
## Exploring a repository
Let's take a look around!

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
## Issues

**Members**
<br />Create an issue:
<br />"Add me as a collaborator!"

**Leaders**
<br />Add your members,
<br />resolve the issues

Note:
* Issues are what drives work
* They describe problems, tasks, etc.
* Anyone can create issues on any repository
* **DEMO:** (Jan) creates an issue to add Jan as collaborator
* Collaborators can make changes, branches and merge in PR's
* Create an issue for your team leader add you as collaborator
* Team leader, add them in the settings page and resolve the issues!
* **DEMO:** Add Jan as collaborator to your demo repo. Resolve the issue   
 
>>>>NEWSECTION
## You've got mail!

Thread subscription
<br />Repository watching

Note:
* Before we really get into things, let's prevent email floods
* GitHub sends you notifications of:
  * Issue threads you're subscribed to
  * Repositories you're watching
  * By default, you watch repositories you join (changed in profile settings)
* You can unsubscribe from issue threads
* You can unwatch repositories
* **DEMO:** Unwatch and unsubscribe from thread/repositories
* **DEMO:** Change notification settings in GitHub profile
    
>>>>NEWSECTION 
## A quick recap

Git(Hub)<br />
Repositories<br />
Collaborators<br />
Issues<br />
Notifications<br />

Note:
* GitHub is a collaboration platform around Git
* Git is a versioning control system used for managing file versions
* Repositories are the heart of a project, they hold the files and are the scope of issues
* Issues are discussion threads for problems/tasks to work on
* Notifications are eager to give you updates on issues, but don't get flooded by them!

>>>>NEWSECTION 
## Proposing a workflow

**[The GitHub Flow](https://guides.github.com/introduction/flow/)**

Note:
* Before we start working, let us propose a nice workflow
* Workflow promoted by GitHub themselves
* Let's take a quick peek
* **DEMO:** Go through GH Flow
* It focuses on tying your work to issues and promotes discussion of the changes you're making

>>>>NEWSECTION                                                                                                                                                      
## Our first contribution

Create an issue!

Note:
* Let's do some work following this flow
* Say we want to add bios of all the team members to the project
* Let's start by creating issues for that, shall we?
* **DEMO:** Create an issue:
  * Title: Create a bio file for Thierry
  * Content: 
    * Add a bio with some info on Thierry
    * Include Steps (Create a branch, add file, create a commit, open a PR, have a discussion about PR, merge PR)
  * Demonstrate markdown for headers, checkboxes, etc.
    * Toolbar
    * `Preview`
  * `Assign` the issue to a person
  * Add a `label`  

>>>>NEWSECTION                                                                                                                                                      
## Our first contribution

Branch off!

Note:                               
* Now we have our issue, let's do some work
* If you work on a branch, your work is isolated and doesn't bother others
* So let's make a branch to do some work
* Briefly discuss "Git Status" toolbar (commits, branches, releases, contributors) 
* **DEMO:** Creating a Branch          
* Create a branch named `thierry-bio`
* Demo what happens when you refresh the page/click on the main repo!
    
>>>>NEWSECTION                                                                                                                                                      
## Our first contribution

Add some data!

*bio/thierry-bio.md*
```
 * name: Thierry
 * from: Belgium
 * likes: Git! 
```

Note:
 - **DEMO:** Create a file in a folder in the repository
     - *bio/thierry-bio.md*
   - When they've all done this, go to the commit graph
   - Explain commits
      - Creates a safe rollback point for us.
      - Allows us to see our repo at a specific point in time.
      - "Oops Button"
      - Even allows us to rollback specific commits

>>>>NEWSECTION
## Our first contribution

Create a pull request!
  
Note:
- Creating Pull Requests
  - Understanding Pull Requests
  - **DEMO:** Creating a Pull Request on GitHub
    - Show `base:` and `compare:` drop downs
    - Issue resolution (Resolves/Closes #issuefrombefore)
    - Assignment, Label
    - Create PR
    - Assign to leader
  - Return to original issue and hover over information pane
  - Summarize where we've been.                            

>>>>NEWSECTION
## Our first contribution
 
Collaborate on a PR, discuss!

Note:
- Pull Request Tools
    - `Conversation` view
    - `Commits` view
    - `Files changed` view
    - Create line comment
    - Add a general comment to the discussion
    - Add :+1: emoji
  - **DEMO:** Comment on someone else's pull request

>>>>NEWSECTION
## Our first contribution

Let's tweak our data!

Note:
- Editing Pull Request Files
  - **DEMO:** Edit the file based on the pull request comments
   - Edit and commit the file changes
   - Show the `Commits` tab  

>>>>NEWSECTION
## Our first contribution

Merge in the branch!

Note:
- Merging Pull Requests
  - What happens when we merge Pull Requests
    - Rule: Only merge your own pull request. Add :ship: to someone else's PR as example.
  - **DEMO:** Merge the pull request, closing the issue in the merge commit
    - Discuss merge dropdown. Squash/Merge vs. default merge.
      - A squash merge deletes commit history. 
    - Merge attempt failed. 
      - "Every time someone merges, GitHub checks for conflicts. If it doesn't have time to make the checks because of the amount of merges, it'll give us a 'Merge Attempt Failed' dialog." 
    - Delete the branch
    - Discuss "Revert"
    - Show the closed issue                                                                            

>>>>NEWSECTION                                                                           
## Another quick recap

* Issue
* Branch
* Commit
* Pull request
* Merge

>>>>NEWSECTION                                                                           
## A local Git

* UI (GitHub Desktop/gitg)
* Terminal

Note:
- Why Use GitHub Desktop?
  - Everything is the same, except that you can't update multiple files in the same commit.
  - Git is super lightweight and you can work locally completely separate from your remote, and offline, with the entire history.
  - Everyone has a back-up at all times. DVCS.  

>>>>NEWSECTION
## Setting up

Note: 
- Intro to Desktop
  - Tutorial Repo (Encourage them to do this later.)
  - Ensure we are logged in.
    - GitHub Desktop Preferences
    - Accounts
    - Login
      - Don't use @github.com, username will work just fine. 
      - Reiterate. This is not a constant connection. It will only do so when we tell it to. 
      - Update Advanced config information. Email is trainingdemos+githubteacher@github.com  

>>>>NEWSECTION 
Note:
- Basic GitHub Desktop Configuration
  - Git Configuration Levels
  - **DEMO + ACTIVITY:** Set basic config  

>>>>NEWSECTION         
Note:
- Cloning a Repository
  - Why we clone
    - Add assumes that you have a local repo and want to look at it using GH Desktop.
    - Create assumes you want to create a repo on your local machine.
    - Clone looks at all of the repos that we have access to. Filter to find the repo that we're looking for.
  - **DEMO:** Clone the repository
    - Click through and demo all changes on visualization tool.
    - Go over "Sync". Makes sure what we're working on is the most recent version.
    - Shows user, time, commit ID, revert, etc.
    - Introduce what we're doing. Return to GitHub flow diagram. Begin again.
    - Create branch on Desktop called `githubteacher-desktop`
      - Typically branch from master.
  - **LAB:** Learner clones the repo and switches to their branch  

>>>>NEWSECTION 
Note:
- Editing Local Files
  - Open and work in Atom
    - No matter where I work on a branch, those changes persist with me.
    - Show branch dialog at bottom of page.
    - Make changes to original file.
    - You can't use Desktop to edit files, you have to use a text editor.
  
>>>>NEWSECTION 
Note:
- Advanced Commits
  - Explain the two stage commit on document on desktop. 
  - **DEMO:** Commit the changes
    - Show un-synced changes. <-- Note the icon differences on the Desktop and un-synced tab.
    - Discuss local vs. remote operations.
    - Create a PR using the button. Allowed to @ mention again.
    - Navigate to .com and you can see multiple commits. 
    - Show file on master without changes
    - Show file on branch with changes
  - **LAB:** Learner edits, saves, and commits file
    - Make two changes to original file and add them as separate commits.
    - Add two files to a commit.  

>>>>NEWSECTION 
Note:
- Publishing Changes
  - Explain publish/sync
  - **DEMO:** Publish changes
    - Create a PR from published changes
  - **LAB:** Learner publishes changes and creates a PR
  - Merge PR
  - Sync again

>>>>NEWSECTION 
Note:
### Merge Conflicts
  - Create a new branch, called conflict-branch.
  - Make changes to your original file.
  - Return to master, make changes to master.
  - Start a PR between master and conflict-branch.
  - Note issue, create PR anyways.
  - Return to Desktop
  - Switch to conflict branch
  - Update from Master button (creates a merge locally)
  - Open with editor.
  - Resolve conflict.
  - Return to desktop. Submit commit.
  - Return to .com, complete PR
  - Discuss merge conflict principles

>>>>NEWSECTION                        
Note:
### Managing Projects on GitHub
- Using pulse
- Using graphs
  - Network shows branches
  - Members shows forks
- Star (bookmarks + showcases)
- Explore (showcases)
