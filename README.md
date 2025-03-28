# Tag, You're Git!
<small>2025-03-28</small>

Welcome to a github collaboration practice project! This is essentially a fun™ exercise designed to help us get more familiar with the collaborative aspects of GitHub (i.e. cloning repositories, making changes, and opening pull requests).

Many of us are comfortable cloning repositories, and making modifications, but often we keep those changes to ourselves.  Few of us get into branching and contributing to other people's code.  Pull requests help you propose changes to the team. They provide a platform for discussion, review, and eventually, integration of changes into the main project. This collaborative workflow is essential in a team setting as it ensures that projects can benefit from the collective expertise of the team.

Let's make sure that we're *choosing* to work on our own, and we're not limited by our ability to work with the collaborative aspects of git.  

 This repository is a public space within the [Maritimes](https://github.com/Maritimes/) github account, and I've added a [Contributor Code of Conduct](CODE_OF_CONDUCT.md) to remind everyone to behave.) 

**Nothing of importance exists here, and no assessments are going to fail if we mess anything up while we're learning.**

## Initial Setup (cloning the repo via RStudio)

Although you can work with this via numerous tools, I'll assume you're working with RStudio for any instructions below.  If you're using some other method, you probably don't need to read any instructions anyways.  :)

Open RStudio and go to File > New Project > Version Control > Git. In the "Repository URL" field, paste the URL of the GitHub repository (https://github.com/Maritimes/Tag_Youre_Git.git). This will clone the repository to your local machine.

## What To Do
Once you've cloned the repo, you can try the following:

1. Create a new branch.
2. Add/change file(s) in the repository. 
3. Commit your changes and push your branch to GitHub.
4. Open a pull request and in the description, tag someone to review your changes (using "@username").
5. The tagged team member will (hopefully) review your changes, merge the pull request, and then repeat the process, tagging the next person in line.

## Opening a Pull Request

1. **Navigate to the main page of the repository**: After you have pushed your changes to your branch on GitHub, navigate to the main page of the repository on GitHub.

2. **Click on 'Pull request'**: On the repository page, click on the 'Pull request' tab. This will take you to the pull request page.

3. **Click on 'New pull request'**: On the pull request page, click on the 'New pull request' button.

4. **Select the branch**: In the 'base:' and 'compare:' dropdown menus, select the branches you want to compare. The 'base:' branch is the one where you want your changes to go, and the 'compare:' branch is the one where you have made changes.

5. **Review your changes**: GitHub will show you the changes you made on your branch compared to the base branch. Review these to make sure everything is correct.

6. **Click on 'Create pull request'**: If everything looks good, click on the 'Create pull request' button.

7. **Fill in the pull request form**: Give your pull request a title and describe your changes in the comment section. If you want to notify a team member to review your changes, type '@' followed by their username.

8. **Submit the pull request**: Click on 'Create pull request' to submit your pull request. Now your team member can review your changes and merge them into the base branch.

## When You Are Tagged
1. In RStudio, go to the "Git" tab and click on "Pull". This will update your local repository with the latest changes from GitHub.
2. In the "Git" tab, click on "New Branch", enter a name for your branch, and click "Create".
3. Make your changes to the file(s) in the repository.
4. Once you're done, go to the "Git" tab in RStudio. You'll see the files you've changed. Check the boxes next to them to stage the changes.
5. In the "Commit message" field, write a brief description of what you've changed. Click "Commit".
6. Click "Push" to push your changes and the new branch to GitHub.
7. Go to the GitHub page for the repository. You'll see a message about your recently pushed branch. Click "Compare & pull request".
8. On the next page, write a description for your changes. In the description, tag the next person to review your changes using "@username". Click "Create pull request".
9. After your changes have been reviewed and merged, you can delete your branch to keep the repository clean. In RStudio, go to the "Git" tab, click on "More", then "Shell...". In the shell, type `git branch -d branch_name` (replace `branch_name` with the name of your branch), then press Enter.

Remember to always pull the latest changes from GitHub before starting work on a new branch. This ensures you're always working with the most up-to-date version of the project.

## When You Need to Review and Merge a Pull Request

1. If someone tags you, you'll receive a notification on GitHub that you've been tagged in a pull request. Go to the repository page on GitHub and click on "Pull requests".
2. Click on the pull request you've been tagged in.
3. Review the changes made. These will be shown under "Files changed".
4. If everything looks good, click "Merge pull request" then "Confirm merge".
5. Now it's your turn to repeat the process starting from step 1 in the "When You Are Tagged" section.

Remember, the goal is to practice and learn. Don't be afraid to ask for help if you're unsure about something. You could use Teams, but rather hassling anyone in particular, I think we have a space we can use here, at the [Gitgub Discussion Board for this repo](https://github.com/Maritimes/Tag_Youre_Git/discussions)

## Participating Without Being Tagged
You can jump in and contribute at any time, even if you haven't been tagged. By tagging someone in your pull request, you're effectively re-starting the game and re-engaging your team in the project.

1. In RStudio, go to the "Git" tab and click on "Pull". This will update your local repository with the latest changes from GitHub.
2. In the "Git" tab, click on "New Branch", enter a name for your branch, and click "Create".
3. Make your changes to the file(s) in the repository.
4. Once you're done, go to the "Git" tab in RStudio. You'll see the files you've changed. Check the boxes next to them to stage the changes.
5. In the "Commit message" field, write a brief description of what you've changed. Click "Commit".
6. Click "Push" to push your changes and the new branch to GitHub.
7. Go to the GitHub page for the repository. You'll see a message about your recently pushed branch. Click "Compare & pull request".
8. On the next page, write a description for your changes. In the description, tag a team member to review your changes using "@username". Click "Create pull request".


## Inviting External Colleagues

1. On the GitHub page for your organization, go to the "People" tab.
2. Click on "Invite member" and enter the GitHub username or email address of the person you want to invite.
3. Once they accept the invitation, they'll be a member of the organization.
4. Next, go to the GitHub page for the specific repository used in the project.
5. Click on "Settings", then "Manage access".
6. Click on "Invite teams or people", and enter the username of the new member.
7. Make sure to set their permission level to "Write", which will allow them to push to the repository, pull requests, and merge pull requests.

## Handling Merge Conflicts

Merge conflicts occur when Git is unable to automatically resolve differences in code between two commits. While they can seem daunting, don't worry - they're a common part of the collaborative coding process. Here's a guide to understanding and resolving some of the most common merge conflicts.

### Common Merge Conflicts

1. Edit/Edit Conflicts: These occur when two people have changed the same lines in a file, or if one person edited a file and another person deleted the same file.
2. Delete/Edit Conflicts: These occur when one person deleted a file while another person was modifying it.
3. Rename/Edit Conflicts: These occur when one person renamed a file and another person modified the same file.

### Resolving Merge Conflicts

1. Identify the Conflict: Git will tell you that a merge conflict has occurred after an attempted git pull. It will also show you the files where conflicts occurred.
2. Examine the Conflict: Open the file with the conflict. Git marks the problematic area in the file by enclosing it in <<<<<<< HEAD and >>>>>>> [other/branch/name]. The changes from the HEAD (your branch) are shown first, followed by the changes from the other branch.
3. Resolve the Conflict: Decide if you want to keep only your branch's changes, keep only the other branch's changes, or make a brand new change, which may be a mix of the two. Delete the conflict markers and make the changes you want in the file.
4. Commit the Resolution: After you've resolved the conflict, stage the file with git add. Then, commit the resolution with git commit.

Remember, when resolving conflicts, communication is key. If you're unsure about how to resolve a conflict, reach out to the person you're collaborating with. It's a team effort!

This guide should help your team understand and resolve the most common types of merge conflicts.

## Conclusion
That's it.  I hope this is useful for people, and maybe even kind of fun.  If you have any suggestions, please let me know!   