# 0x01. Git

#### About: Git, Code versioning, Github

### Resources
#### Read or watch:
* [Resources to learn Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
* [About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
* [How to write a Git commit message](https://cbea.ms/git-commit/)
#### Additional Resources:
* [Learning branching](https://learngitbranching.js.org/)
* [Effective pull requests and other good practices for teams using GitHub](https://codeinthehole.com/tips/pull-requests-and-other-good-practices-for-teams-using-github/)

### Learning Objectives
- What is source code management
  <p>Ans: Source Code Management is a process or tool used to keep track of changes to the code files in a source code repository</p>
- What is Git
  <p>Ans: Git is like a tool (a version control) that helps developers keep track of changes they make to their files while working on a project. It allows them to work on their own local machines and save their changes even without an internet connection. Git is powerful and flexible, but it doesn't have a fancy interface.</p>
- What is GitHub
  <p>Ans:  GitHub is a website that takes Git and adds some extra features to make it easier to collaborate with others. It acts as a central place where developers can store their Git projects and work together. It provides a nice web-based interface for managing and sharing code, tracking issues, and reviewing changes. GitHub makes it easier for people to work together on coding projects..</p>
- What is the difference between Git and GitHub
  <p>Ans: Git is the behind-the-scenes tool that tracks changes, while GitHub is a user-friendly website built around Git that makes it easier for people to work together on code projects.</p>
- How to create a repository
  <p> Ans: <br />
    1. Sign in to your GitHub account <br />
    2. Once you're logged in, click on the "+" icon in the top-right corner of the GitHub interface. Then select "New repository" from the dropdown menu. <br />
    3. On the "Create a new repository" page, provide neccesary informations (Repository name, Description, Public or private, license) <br />
    4. Once you have entered the necessary information, click on the "Create repository" button. 
    5. Congratulations! You have successfully created a repository on GitHub. The repository page will be displayed, showing the repository details and options.
  </p>
- What is a README
  <p>Ans: A README is like a guidebook or manual for a software project. It's a file that provides important information and instructions about the project. It tells you what the project is about, how to set it up on your computer, how to use it, and any special things you need to know. It's like having a helpful document that explains everything you need to know about the project, kind of like a user manual.</p>
- How to write good READMEs
  <p>Ans: A good README must be Concise, Have a Project description, have an Installation instructions, have a Usage examples, explain the relevant settings and options users can modify, have a Documentation, have Contributions and license, with Contact informations and be formatted nicely. </p>
- How to write helpful commit messages 
  <p> When writing commit messages: <br />
    1. Keep them short and concise, ideally under 50 characters.<br />
    2. Start with an action verb to clarify the purpose (e.g., Add, Fix, Update). <br />
    3. Be specific about the changes and their reasons. <br />
    4. Include relevant context, like issue references. <br />
    5. Separate the subject line from the optional body.
  </p>
- How to push code
  <p> Make sure you have a local Git repository set up. <br />
    1. Add and commit your changes using git add and git commit. <br />
    2. Link your local repository to the remote repository using git remote add origin <remote repository URL>. <br />
    3. Push the code with git push -u origin <branch>, replacing <branch> with the branch name. <br />
    4. Enter your credentials if prompted.
  </p>
- How to pull updates
  <p> Guide: 
    1. Make sure you are in your project directory using the command-line interface.<br />
    2. Check for any uncommitted changes using git status. Commit or stash them if necessary.<br />
    3. Fetch the latest changes from the remote repository: git fetch.<br />
    4. Merge the fetched changes into your local branch: git merge origin/<branch>.<br />
    5. Resolve any conflicts, if encountered.<br />
    6. Add the modified files: git add <file> or git add ..<br />
    7. Commit the changes: git commit -m "Merge changes from remote repository".<br />
    -- Congratulations! You have successfully pulled the latest updates.
   </p>
- How to create a branch
  <p> Guide: <br />
    1. Open your command-line interface and navigate to your Git repository's directory.<br />
    2. Use the command: git branch <branch-name> to create a new branch. Replace <branch-name> with the desired name for your branch.<br />
    3. To switch to the newly created branch, use the command: git checkout <branch-name>.<br />
    -- That's it! You have successfully created and switched to a new branch.
  </p>
- How to merge branches
  <p> Guide: <br />
    1. Switch to the branch you want to merge the changes into: git checkout <target-branch>.<br />
    2. Execute the merge command: git merge <source-branch>. This combines the changes from the source branch into the target branch.<br />
    3. Resolve any conflicts if they occur.<br />
    4. Add the modified files: git add <file> or git add ..<br />
    5. Commit the merge changes: git commit -m "Merge <source-branch> into <target-branch>".
  </p>
- How to work as collaborators on a project
  <p> Guide: <br />
    1. Set up a shared repository on a platform like GitHub.<br />
    2. Clone the repository to your local machine using git clone <repository URL>.<br />
    3. Create and switch to separate branches for your work using git branch <branch-name> and git checkout <branch-name>.<br />
    4. Make changes to the codebase on your branch.<br />
    5. Commit your changes using git add <file> and git commit -m "Descriptive message".<br />
    6. Push your branch to the remote repository using git push origin <branch-name>.<br />
    7. Review and merge each other's branches using pull requests or merge requests on the platform.<br />
    8. Regularly pull updates from the main branch using git pull origin <main-branch>.<br />
    9. Resolve any conflicts that may arise during merging by editing the conflicting files and committing the changes.
  </p>
#### By following these steps, collaborators can efficiently work together on a project, contributing changes, reviewing each other's work, and merging their contributions to create a cohesive codebase.
- Which files should and which files should not appear in your repo 
  <p>Files that should appear in your repo: <br />
      Source code files (e.g., .java, .py, .cpp) <br />
      Configuration files (e.g., .json, .xml, .yaml)README and documentation files (e.g., README.md)Build files (e.g., Makefile, build.xml, pom.xml) <br />
      Dependency files (e.g., package.json, requirements.txt, Gemfile)
    </p>
  <p>Files that should not appear in your repo: <br />
    Compiled or generated files (e.g., .class, .jar, .war) <br />
    Build output directories (e.g., /target, /bin, /dist)<br />
    System-specific files (e.g., .DS_Store, thumbs.db, .idea)<br />
    Credentials or sensitive information files (e.g., passwords, access tokens)
  </p>
#### By including the necessary files and excluding unnecessary or sensitive files, you can maintain a clean and focused repository.
## Basic Usage:
```bash
$ git clone <repo> (for cloning repo locally/from the terminal)
$ touch test (create an empty file named test)
$ git add test (adds a change in the working directory to the staging area)
$ git commit -m "Initial commit" (recording changes with a name/message)
$ git push origin main (sends the recent commit history from your local repository to GitHub)
```
  
