### GIT AND GITHUB NOTES

## What is version control?

Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later. This allows you to revert files back to a previous state, compare changes over time, and see who last modified something that might be causing a problem. Version control systems are most commonly used in software development and allow developers to easily collaborate on code.

## Git Version Control explain in details?

Git Version Control is a distributed version control system that is used to track changes in computer files and coordinate work on those files among multiple people. It is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

Git stores and manages changes to a project in a data structure called a repository. Each repository contains a full history of all changes made to the project, along with who made the changes and when. This allows developers to easily track changes, undo mistakes, and collaborate with other developers on the project.

The repository also stores information about each file, such as when it was created, when it was last modified, and who made the changes. This information is stored in a data structure called a “commit”. Each commit contains a snapshot of the project at a particular point in time. This allows developers to easily compare different versions of the project and revert back to older versions if needed.

Git also makes it easy for developers to collaborate on a project. Developers can create “branches” of the project, allowing them to work on different versions of the project in parallel. This allows developers to collaborate on a project without risking interfering with each other

## What are Pull Requests? How do you make them?

Pull Requests are a way to submit changes to a project on Github. They are a request for someone else to review and then approve or reject the changes. To make a pull request, you must first create a branch off of the main project, make the changes you want on the branch, then push the branch to Github. Next, you must create a pull request on Github. This will open a discussion about the changes you made and allow others to review and comment on them. Finally, once the pull request is approved, the changes will be merged into the main project.

## What is merging in git?

Merging in Git is a process of combining different sequences of commits into one unified branch. It is typically used to integrate changes from two distinct branches. Merging in Git is usually performed by combining the separate branches into a single branch in a repository. This helps to keep track of the changes in the codebase and also makes it easier for developers to collaborate on a project.

## How to create branches, why do we do that?

Creating branches is an important part of a successful version control system. Branches allow developers to work on different versions of a project simultaneously without affecting the main or master branch. Branches are created so that developers can create new features, bug fixes, or experiments without affecting the main codebase. This allows for a much more organized and efficient development process.

## What is commiting?

Committing is a process in version control systems such as Git. It is the action of saving changes to a file or set of files to the repository. Committing is the act of taking the changes you've made and marking them for inclusion in the project's history. This allows other developers to review the changes, and then decide if they should be incorporated into the project

## How can you amend a message of git commit?

You can amend a Git commit message by running the command 'git commit --amend' and then entering the new commit message.

## What is .gitignore, why do we need it?

.gitignore is a file used to tell git which files or folders to ignore when committing code to a repository. This is useful for files that contain sensitive information, like passwords, or files that are not needed for the project, like compiled files. By using a .gitignore file, these files will not be committed to the repository and will remain private.

## What is a merge conflict? how do we resolve it?

A merge conflict occurs when two different branches of a repository contain different versions of the same file and a user attempts to merge the branches together. This can occur when two different users have edited the same file, and the user attempting to merge the branches has to pick which version of the file to save. To resolve a merge conflict, the user should review the conflicting changes, decide which changes to keep, and then manually edit the file to include all of the desired changes.

## How do you see previous logs in github?

You can view previous logs in GitHub by navigating to the repository's "Commits" page. From there, you can view a list of all the commits that have been made to the repository, along with the message associated with each commit, the date and time of the commit, and other relevant information.

## How do you clone a repository?

1. Go to the repository you'd like to clone.
2. Click the "Clone or Download" button on the repository page.
3. Copy the clone URL for the repository.
4. Open the command line and change the current working directory to the location where you want the cloned directory to be made.
5. Type git clone, and then paste the URL you copied in Step 2.
6. Press Enter. Your local clone will be created.

## How do you fork a repository? What is the difference between cloning and forking?

1. To fork a repository, click on the “Fork” button located in the top-right corner of the repository page.

2. The difference between cloning and forking is that when you clone a repository you get a local copy of the entire repository, including all the versions and branches. When you fork a repository, you create a copy of the original repository in your own GitHub account, allowing you to make changes to the repository without affecting the original.

## Who created git? What are some platforms other than github to use version control?

Git was created by Linus Torvalds in 2005.

Some platforms other than GitHub to use version control include Bitbucket, GitLab, and SourceForge.

## What is github actions?

GitHub Actions is a feature of GitHub that allows users to create custom software development lifecycle workflows directly in their GitHub repository. It gives users the flexibility to build, test, package, release, and deploy any project on GitHub. With GitHub Actions, developers can automate their workflows, integrate external tools, and access rich data about the code they’re managing, all within their reposi.

## How can you deploy to vercel or netlify from github actions?

You can deploy to Vercel or Netlify from Github Actions using the Vercel or Netlify Action for Github. You can create a workflow that runs when a push is made to your repository and uses the action to deploy your site to the chosen hosting platform. This can be configured to run on any branch you choose.

## What is CI CD?

CI/CD stands for Continuous Integration/Continuous Delivery. It is a DevOps practice that enables software teams to quickly and reliably deliver software updates to customers. CI/CD automates the process of building, testing, and deploying software updates, making it much easier for teams to rapidly deliver new features, bug fixes, and other updates.

## Why is git add . a bad idea and not recommended?

Git add . is not recommended because it will add all files and changes in the current directory, including untracked and ignored files. This can lead to unintentional staging or committing of unwanted or ignored files, which could potentially cause problems and errors with your repository.

## What happens when you have a git repository inside another repository and you try to add new commits?

If you have a git repository inside another repository, it will be treated like any other file or folder inside the outer repository. When you add new commits to the inner repository, they will be added to the outer repository as well, just like any other changes. However, the commits will not be tracked by the outer repository, since it does not recognize the inner repository as part of its version control system.
