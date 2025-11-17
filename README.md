# Tag, You're Git!
<small>2025-11-17</small>

Welcome to a github collaboration practice project! This is essentially a fun™ exercise designed to help us get more familiar with the collaborative aspects of GitHub (i.e. forking repositories, making changes, and opening pull requests).

Many of us are comfortable cloning repositories and making modifications, but often we keep those changes to ourselves. Few of us get into branching and contributing to other people's code. Pull requests help you propose changes to the team. They provide a platform for discussion, review, and eventually, integration of changes into the main project. This collaborative workflow is essential in a team setting as it ensures that projects can benefit from the collective expertise of the team.

People can find themselves working on a team that uses git/github, and the only repository they use is core to the work of their unit - it is not an appropriate place to "move fast and break things".  That's where this repository comes in - **nothing important exists in this repo, and no core work is going to fail as a result of anything we do in here**.  Please feel free to add/remove/edit any files you want (but note that I've added a [Contributor Code of Conduct](CODE_OF_CONDUCT.md) to remind everyone to behave).

Let's make sure that we're *choosing* to work on our own, and we're not limited by our ability to work with the collaborative aspects of git.

## Initial Setup (forking and cloning via RStudio)

Although you can work with this via numerous tools, I'll assume you're working with RStudio for any instructions below. If you're using some other method, you probably don't need to read any instructions anyways. :)

**Fork the repository:**

1. Go to https://github.com/Maritimes/Tag_Youre_Git
2. Click the "Fork" button in the upper right corner
3. This creates a copy of the repository under your own GitHub account

**Clone your fork:**

Open RStudio and go to File > New Project > Version Control > Git. In the "Repository URL" field, paste the URL of **your forked repository** (it will be https://github.com/YOUR-USERNAME/Tag_Youre_Git.git). This will clone your fork to your local machine.

## What To Do
Once you've cloned your fork, you can try the following:

1. Create a [new branch](#about-branching).
2. Add/change file(s) in the repository.
3. Commit your changes and push your branch to **your fork** on GitHub.
4. Open a pull request from your fork to the original repository and in the description, tag someone to review your changes (using "@username").
5. The tagged team member will review and comment on your changes. The repository maintainer will then merge the pull request if approved.

## About Branching

Branches are parallel versions of your repository that allow you to work on different tasks simultaneously without interfering with each other. Think of the main branch as the stable, production-ready version of your code, while other branches are workspaces for development.

**Why use branches?**

Branches let you isolate your work. If you're refactoring a major function but discover a critical bug that needs immediate attention, you can:
1. Commit your refactoring work on its current branch
2. Switch back to the main branch
3. Create a new branch for the bugfix
4. Fix the bug and merge it to main
5. Return to your refactoring branch and continue working

Without branches, you'd have to either abandon your refactoring progress or push untested, incomplete code along with your bugfix.

**Branch naming conventions:**

Use descriptive names that indicate the purpose of the branch. Common patterns include:
- `feature/add-data-validation`
- `bugfix/correct-date-parsing`
- `hotfix/security-patch`
- `yourname/experiment-with-new-approach`

This makes it easy for others (and future you) to understand what each branch is for at a glance.

## Opening a Pull Request

1. **Navigate to your fork**: After you have pushed your changes to your branch on your fork, navigate to your fork's page on GitHub.

2. **Click on 'Contribute'**: You'll see a "Contribute" button near the top of the page. Click it, then click "Open pull request".

3. **Review the branches**: GitHub will automatically set the base repository to `Maritimes/Tag_Youre_Git` and base branch to `main` (or `master`), and compare it to your fork and branch. Verify these are correct.

4. **Review your changes**: GitHub will show you the changes you made on your branch compared to the base branch. Review these to make sure everything is correct.

5. **Click on 'Create pull request'**: If everything looks good, click on the 'Create pull request' button.

6. **Fill in the pull request form**: Give your pull request a title and describe your changes in the comment section. If you want to notify a team member to review your changes, type '@' followed by their username.

7. **Submit the pull request**: Click on 'Create pull request' to submit your pull request. Now others can review and comment on your changes.

## When You Are Tagged in a Pull Request

When someone tags you in a pull request, they're asking you to review their proposed changes. Here's what to do:

**As a Reviewer (anyone can do this):**

1. **Check notifications**: You'll receive a notification on GitHub. Go to the original repository page (https://github.com/Maritimes/Tag_Youre_Git) and click on "Pull requests".

2. **Review the changes**: Click on the pull request you've been tagged in. Review the changes under "Files changed". Consider:
   - Does the code make sense?
   - Will it break anything?
   - Is the purpose clear?

3. **Provide feedback**: Use GitHub's review features to leave comments on specific lines if you have questions or suggestions. You can click "Approve" to indicate the changes look good, or "Request changes" if issues need addressing.

4. **Participate in discussion**: Engage in the conversation. Ask questions, make suggestions, learn from others' approaches.

**As the Repository Maintainer (merging):**

Only the repository owner or designated collaborators can actually merge pull requests. If you have merge access:

1. **Review feedback**: Check that any issues raised by reviewers have been addressed.

2. **Merge the pull request**: Once satisfied with the changes and any review comments, click "Merge pull request" then "Confirm merge".

3. **Continue the chain**: After merging, follow the steps in "When You Want to Contribute" to make your own changes and tag the next person.

## When You Want to Contribute

You can jump in and contribute at any time, whether you've been tagged or not. By tagging someone in your pull request, you're engaging your team in the project.

1. **Sync your fork**: Go to your fork on GitHub. If it's behind the original repository, you'll see a message. Click "Sync fork" then "Update branch" to bring your fork up to date.

2. **Pull latest changes**: In RStudio, go to the "Git" tab and click on "Pull". This will update your local repository with the latest changes from your fork.

3. **Create a new branch**: In the "Git" tab, click on "New Branch", enter a name for your branch, and click "Create".

4. **Make your changes**: Make your changes to the file(s) in the repository.

5. **Stage and commit**: Go to the "Git" tab in RStudio. Check the boxes next to changed files to stage them. Write a commit message and click "Commit".

6. **Push to your fork**: Click "Push" to push your changes to your fork on GitHub.

7. **Open a pull request**: Go to your fork's GitHub page. You'll see a message about your recently pushed branch. Click "Compare & pull request".

8. **Tag someone**: Write a description for your changes and tag a team member using "@username". Click "Create pull request".

9. **Clean up**: After your changes have been merged into the original repository, you can delete your branch to keep things tidy. In RStudio, go to the "Git" tab, click on "More", then "Shell...". In the shell, type `git branch -d branch_name` (replace `branch_name` with the name of your branch), then press Enter.

Remember to always sync your fork and pull the latest changes before starting work on a new branch. This ensures you're always working with the most up-to-date version of the project.

## Adding Collaborators (Optional - For Repository Owners)

If you want to give someone direct write access to the repository (bypassing the fork workflow), you can add them as a collaborator:

1. Go to the repository page on GitHub.
2. Click on "Settings", then "Collaborators and teams".
3. Click "Add people" and enter their GitHub username.
4. Set their permission level to "Write" or higher.

Note: This is optional. The fork workflow described above works for anyone without requiring you to add them first. Collaborators can merge pull requests, while non-collaborators can only submit and review them.

## Handling Merge Conflicts

Merge conflicts occur when Git is unable to automatically resolve differences in code between two commits. While they can seem daunting, don't worry - they're a common part of the collaborative coding process. Here's a guide to understanding and resolving some of the most common merge conflicts.

### Common Merge Conflicts

1. Edit/Edit Conflicts: These occur when two people have changed the same lines in a file, or if one person edited a file and another person deleted the same file.
2. Delete/Edit Conflicts: These occur when one person deleted a file while another person was modifying it.
3. Rename/Edit Conflicts: These occur when one person renamed a file and another person modified the same file.

### Resolving Merge Conflicts

1. **Identify the Conflict**: Git will tell you that a merge conflict has occurred after an attempted git pull. It will also show you the files where conflicts occurred.

2. **Examine the Conflict**: Open the file with the conflict. Git marks the problematic area in the file by enclosing it in `<<<<<<< HEAD` and `>>>>>>> [other/branch/name]`. The changes from the HEAD (your branch) are shown first, followed by the changes from the other branch.

3. **Resolve the Conflict**: Decide if you want to keep only your branch's changes, keep only the other branch's changes, or make a brand new change, which may be a mix of the two. Delete the conflict markers and make the changes you want in the file.

4. **Commit the Resolution**: After you've resolved the conflict, stage the file with git add. Then, commit the resolution with git commit.

Remember, when resolving conflicts, communication is key. If you're unsure about how to resolve a conflict, reach out to the person you're collaborating with. It's a team effort!

This guide should help your team understand and resolve the most common types of merge conflicts.

## Need Help or Have Questions?

If you run into issues, have questions about the workflow, or want to discuss Git/GitHub topics, use the [Discussion Board](https://github.com/Maritimes/Tag_Youre_Git/discussions) for this repository.

**Use Discussions for:**
- Questions about forking, branching, or pull requests
- Troubleshooting problems you encounter
- Suggestions for improving this practice repository
- General Git/GitHub questions and tips

**Don't use Discussions for:**
- Code review feedback (use pull request comments instead)
- Commenting on specific changes (use pull request comments instead)

The Discussion Board is a collaborative space where we can all learn from each other. Don't hesitate to ask questions or share what you've learned!

## Conclusion

That's it. I hope this is useful for people, and maybe even kind of fun. If you have any suggestions, please let me know!