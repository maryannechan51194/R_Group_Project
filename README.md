# R_Group_Project
MITB R Group Project
GETTING STARTED — SET UP REPO & COLLABORATORS
Assign a Repo Owner: This person should be in charge of creating the repo, adding collaborators, and overseeing pull requests.
Create Repository: The owner. should create a new Github repository called on his or her Github profile (ie there should only be ONE Github repo for the entire group)
Add Project to Repo: The leader can create a new directory on her local terminal. The leader can switch (cd) into this directory, and add the directory to the Github repository. See detailed instructions here.
Add Collaborators: The leader invites teammates to work on that repository as Collaborators. To do this, navigate “Settings” -> “Collaborators” from the Github repository. Collaborators should check their email for an invitation to collaborate and accept.
Clone (Don’t Fork) Repo: Each collaborator should clone the repo onto his or her local environment.
BRANCHING
Collaborators should not work directly in the master branch unless to merge with master. The master branch is the default branch that reflects a production-ready state. Instead, collaborators should create their own branches for each task / feature.
For example, if you and your teammates were writing a paper on the history the United States and you each needed to write a paragraph on a given time period, rather than all writing in the same document, you each write your own paragraph in a separate document and then add each paragraph to a “master” document.
Here’s what this translates to in Github.
Working branches: In terminal, each person runs “git branch <branch_name>” ie “git branch feature_1” & “git branch feature_2.” This creates a new version of the master branch.
git branch <branch_name>
2. Integration Branch: Some developers opt to merge features into an “integration branch” instead of master. Consider having the leader generate a third branch called “integration_branch”.
git branch integration_branch
3. SWITCH OUT OF INTEGRATION / MASTER: As stated above, do not work directly in master or integration. I repeat. DO. NOT. WORK. DIRECTLY. IN. MASTER. To switch into your working branches, run “git checkout <name_of_branch> ie “git checkout feature_1”. Forgot your branch name? Run “git branch -a” for a list of all branches. To double check which branch you are in, run “git branch.”
git branch -a
git checkout <branch_name>
git branch
SAVE YOUR CHANGES
As you make changes to your local (desktop) branch, you need to track and stage these changes (snapshotting) so that they can get pushed up to your remote (online) branch. Do this often so that you can still access your changes online in case something happens to your computer!
I remember these steps as “SACP”.
git status: Displays differences between local and remote branch. The Command is “git status”
git status
2. git add: Adds changes in the working directory to the staging area to be include updates to a particular file in the next commit. Command “git add . ” adds all changes to be staged.
git add .
3. git commit: Records changes. Command is “git commit -m <message here>”. Your message should include a description of the changes you made.
git commit -m "My first commit"
4. git push: Pushes the changes to the remote branch, thereby updating it.
git push
ADD YOUR TEAMMATES CHANGES
Your teammate has added new code to the remote integration branch. Pull down this code to your local working branch using the below steps.
Stay in your Local Working Branch
Pull Changes: Pull down the Origin Integration Branch into Local Working Branch: Run “git pull origin <integration_branch>.”
git pull origin <integration_branch>
2. Resolve Merge Conflicts: Choose which conflicting code to add or remove from your local working branch.
3. Save Changes: Save & run git add, commit, push
MERGE YOUR CHANGES INTO INTEGRATION USING TERMINAL
Merging the integration and working branches should occur frequently. The less often you merge, the more merge conflicts you are likely to run into.
At this point, your working branches are up to date, but your integration branches do not reflect the changes you made. To add them, do the following:
Switch into Local Integration Branch:
git checkout <integration_branch>
Pull Features into Integration: Run “git pull origin <working_branch>” This pulls down the commits made on your remote working branch to the local integration branch.
git pull origin <working_branch>
Update Remote Integration Branch: Don’t forget to add, commit & push to update your remote integration branch.
MERGING USING GITHUB UI
This is a visually-friendly point and click approach. Check out this repo as an example
Select a Branch: On the remote repository, you can view the latest commits from each branch. Begin by selecting a branch from the Code tab.

2. Open a Pull Request: Select the branches to merge with & click “Create pull request”

3. Resolve Merge Conflicts (if any). Luckily thee are none!
4. Merge. Click on “Merge pull Request”

4. Pull down the remote integration branch into your local branch.
RESOLVING MERGE CONFLICTS
I recommend doing this together if possible. To reduce merge conflicts, collaborators should avoid the following working on the same files at the same time.
See here for instructions on how to resolve merge conflicts.
CHECK YOUR WORK
Check your work with team to ensure that it reflects the changes.
Spot check files where new changes are expected to be found.
On the github repository, click on “Insights”->”Network” to view the branch history.

PRACTICE
Create a dummy repo and branches to practice in!!
