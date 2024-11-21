# Team Collaboration Project

Welcome to our team collaboration project! This is a fun exercise designed to help us get more familiar with GitHub, specifically the process of cloning repositories, making changes, and opening pull requests. If anything looks duplicated or otherwise unclear, please correct it and provide a quick summary of any changes made.

## How It Works

1. Clone this repository to your local machine.
2. Create a new branch.
3. Make some changes to the file(s) in the repository. Be creative!
4. Commit your changes and push your branch to GitHub.
5. Open a pull request and in the description, tag a team member to review your changes (using "@username").
6. The tagged team member will review your changes, merge the pull request, and then repeat the process, tagging the next person in line.

Remember, the goal is to practice and learn, so don't be afraid to make mistakes. Let's have fun with this!

## Forking vs Collaborating

You may be used to forking repositories, making modifications, and keeping those changes to yourself. This approach is great for personal projects or when you want to experiment with a codebase without affecting the original project. However, in a collaborative environment, it's crucial to share your changes and improvements with the team. That's where branching and pull requests come in.

Unlike forking, which creates a separate copy of the entire repository, branching allows you to isolate your changes within the same repository. This makes it easier for others to review your changes and incorporate them into the main project.

Pull requests are the mechanism for proposing your changes to the team. They provide a platform for discussion, review, and eventually, integration of your changes into the main project. This collaborative workflow is essential in a team setting as it ensures everyone's contributions are recognized and the project benefits from the collective expertise of the team.

So, while forking has its place, branching and pull requests are the tools that truly enable collaboration and shared progress in a project. Let's embrace this approach in our team collaboration project!

## Initial Setup

Open RStudio and go to File > New Project > Version Control > Git. In the "Repository URL" field, paste the URL of the GitHub repository. This will clone the repository to your local machine.

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

1. You'll receive a notification on GitHub that you've been tagged in a pull request. Go to the repository page on GitHub and click on "Pull requests".
2. Click on the pull request you've been tagged in.
3. Review the changes made. These will be shown under "Files changed".
4. If everything looks good, click "Merge pull request" then "Confirm merge".
5. Now it's your turn to repeat the process starting from step 1 in the "When You Are Tagged" section.

Remember, the goal is to practice and learn. Don't be afraid to ask for help if you're unsure about something. Happy coding!

## Participating Without Being Tagged

1. In RStudio, go to the "Git" tab and click on "Pull". This will update your local repository with the latest changes from GitHub.
2. In the "Git" tab, click on "New Branch", enter a name for your branch, and click "Create".
3. Make your changes to the file(s) in the repository.
4. Once you're done, go to the "Git" tab in RStudio. You'll see the files you've changed. Check the boxes next to them to stage the changes.
5. In the "Commit message" field, write a brief description of what you've changed. Click "Commit".
6. Click "Push" to push your changes and the new branch to GitHub.
7. Go to the GitHub page for the repository. You'll see a message about your recently pushed branch. Click "Compare & pull request".
8. On the next page, write a description for your changes. In the description, tag a team member to review your changes using "@username". Click "Create pull request".

This way, you can jump in and contribute at any time, even if you haven't been tagged. By tagging someone in your pull request, you're effectively re-starting the game and re-engaging your team in the project.

## Inviting External Colleagues

1. On the GitHub page for your organization, go to the "People" tab.
2. Click on "Invite member" and enter the GitHub username or email address of the person you want to invite.
3. Once they accept the invitation, they'll be a member of the organization.
4. Next, go to the GitHub page for the specific repository used in the project.
5. Click on "Settings", then "Manage access".
6. Click on "Invite teams or people", and enter the username of the new member.
7. Make sure to set their permission level to "Write", which will allow them to push to the repository, pull requests, and merge pull requests.

## Participating in the Project

The external colleague should follow the "Initial Setup" instructions to clone the repository and set it up in RStudio.

They can then follow the "Participating Without Being Tagged" instructions to create a new branch, make changes, and open a pull request.

In the pull request description, they can tag a member of the organization to review their changes.

This way, you can ensure that external colleagues have the necessary permissions to fully participate in the project.

## Requesting to Join the Project

If you're not part of the organization and haven't been invited, but you're interested in joining the project, here's what you can do:

1. Fork the Repository: Since the repository is public, you can create a fork of it in your own GitHub account. This gives you a copy of the repository that you can clone and work on.
2. Make Some Changes: Clone the repository to your local machine, create a new branch, and make some changes. This could be fixing a bug, adding a new feature, improving the documentation, or any other contribution you think would be valuable.
3. Open a Pull Request: Push your changes to your fork and open a pull request in the original repository. In the pull request description, explain your changes and express your interest in joining the project.
4. Wait for Review: The repository maintainers will review your pull request. If your changes are approved, they'll be merged into the project.
5. Request to Join: After making a contribution, you can request to join the organization. Contact a member of the organization, such as the repository owner, and express your interest in joining. They can then send you an invitation to join the organization.

Remember, open source projects thrive on collaboration and contributions from a diverse range of people. Don't be shy about expressing your interest and making a contribution!

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