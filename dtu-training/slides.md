# DST4L
## Collaborating through GitHub
Jan Krag & Thierry Lacour

>>>>NEWSECTION
## Who are we?
### Jan Krag
<img src="img/jan.png" alt="Jan Krag" width="30%"/>

Continuous Improvement Agent
                  
>>>>NEWSECTION
## Who are we?
### Thierry Lacour
<img src="img/thierry.png" alt="Thierry Lacour" width="30%"/>

Automation Toolsmith
                    
>>>>NEWSECTION
## Who are you?
### Librarians
<img src="img/librarian.jpg" alt="The Librarian" width="30%"/>

Not our typical audience!

>>>>NEWSECTION
## Roadmap
* Hands-on introduction to GitHub
* @lakruzz powertalk
* Terminal ?
* Katas ?

>>>>NEWSECTION
## Setup
Make teams! 
* 3-4 members
* A leader         
* A name

Note:
Have team leads announce team names
                
>>>>NEWSECTION
## Setup
Log in to [github.com](github.com) and...

**Leaders**
* Go to [the training repository](?)
* Fork it!

**Members**
* Go to your leader's repository
 
Note:
  - Ensure students have .com accounts
  - **DEMO:** Fork the repository yourself
                    
>>>>NEWSECTION
## Quick intro
What is ...
* Git?
* GitHub?
* a Git repository?

Note:
  - What is Git?
  - What is GitHub?
  - Briefly explain repos
  - The GitHub Ecosystem
    - Talk about fun open source stuff!
    
>>>>NEWSECTION
## Exploring the repository
Let's take a look around!

Note:
- Exploring a Repository
  - **DEMO:** Exploring a repository
    - `Code` <-- The bulk of your repository, where you keep all your files and data
    - `README.md` <-- A 'Markdown' file which gets rendered on the main page by default, explain markdown
    - `Issues` <-- The heart of collaboration & communication, issues is where you can manage work/report problems,...
    - `Pull Request` <-- Pull requests are a means of proposing changes to the repository, the owner can merge them in
    - `Wiki` <-- "A place to hold documentation for your repo"
    - `Pulse` and `Graphs` <-- "Dashboards, or the stats of your projects. Keep up to date on your project."
    - `Settings` <-- "You don't see this because you aren't an owner or admin of this repository."  

>>>>NEWSECTION
## Issues

**Members**
* Create an issue:
 
"Add me as a collaborator!"

**Leaders**
* Add your members
* Resolve the issues

Note:
  - Using Issues
    - Describe Issues
    - **DEMO:** Using Issues
      - Create issue for "Add me as a collaborator!"
      - Discuss Permissions
        - If you aren't a collaborator, on a public repo you may add a comment to an issue, or create an issue of your own. 
        - You can't create branches, PRs, merge PRs.
    - **DEMO:** Add co-teachers as collaborators to your demo fork. Resolve the issue   
 

>>>>NEWSECTION
## You've got mail!

Notification settings

Note:
- Social Features of GitHub
  - Explain how to control the flood of email by:
    - Unsubscribing to threads
    - Watching (un-watching) repositories
      - Every time you're added as a collaborator to a repo, you're set to watch that repo.
    - Notification settings
    - Notification center (Web icon)
    
>>>>NEWSECTION 
## A quick recap

* Git(Hub)
* Repositories
* Collaborators
* Issues
* Notifications

Now let's get started!

Note:
 - Quickly recap what already went over

>>>>NEWSECTION 
## Proposing a workflow

**[The GitHub Flow](https://guides.github.com/introduction/flow/)**
Note:
 -They'll be making pull requests from their leaders' repo, to their leaders' repo

>>>>NEWSECTION                                                                                                                                                      
## Our first contribution

Create an issue!

Note:
-  TODO: do we want them to create an issue beforehand? I think yes.
- **DEMO & LAB:** 
  - Create an issue
    - Title: Create a bio file for Thierry
    - Content: 
      - Add a bio with some info on Thierry
      - Include Steps (Create a branch, add file, create a commit, open a PR, have a discussion about PR, merge PR)
    - Demonstrate markdown for headers, checkboxes and emoji
      - Toolbar
      - `Preview`
    - `Assign` the issue to the person
    - Add a `label`  

>>>>NEWSECTION                                                                                                                                                      
## Our first contribution

Branch off!

Note: 
- Using Branches
  - Briefly discuss "Git Status" toolbar (commits, branches, releases, contributors)
  - **DEMO:** Creating a Branch
    - Create a branch named `name-bio.md`
  - Notice what happens when you refresh the page/click on the main repo!
    
>>>>NEWSECTION                                                                                                                                                      
## Our first contribution

Add some data!

*bio/thierry-bio.md*
```
name: Thierry
from: Belgium
likes: Git! 
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
Note:
### Using GitHub Locally
- navigate to https://desktop.github.com/
- Why Use GitHub Desktop?
  - Everything is the same, except that you can't update multiple files in the same commit.
  - Git is super lightweight and you can work locally complete separate from your remote, and offline, with the entire history.
  - Everyone has a back-up at all times. DVCS.  

>>>>NEWSECTION 
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
