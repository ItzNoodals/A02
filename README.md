# Part 1: How to Setup your Github Account and Connect with Git (Git Bash)
## Step 1: Account Creation and Repository Setup
1. Go to https://github.com/ and create a free account with any email of your choice.
2. When you account has been made, you will be sent to your dashboard where you can see a green plus (+) button.
3. The green plus (+) button will allow you to create a repository with a name of your choice. For example "First Repo".
4. They will then ask if you will like the repository public or private. Public allows for anyone to see, while private allows for you to see only unless you invite someone.
5. Once that is selected, you select to have a README file be added as well and click create repository.
6. You have now created your first repository.
## Step 2: Downloading and Setting up Git 
1. Go to the official Git website and download and install Git. If you have windows use this link https://git-scm.com/install/windows.
2. The Windows installer will automatically have a Unix-like command-line environment called Git Bash installed.
3. Once you install Git and Git Bash, you will have to first configure your Git Indentity first using the commands:
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
This will allow you to make commits on any repository you work on, on your computer.
4. Use the command "git config --global init.defaultBranch main" to allign with Git Hub standards
5. Once that is all done, you can now start to clone your first repository.
## Step 3: Cloming Your Remote Repository
1. On your Git Hub dashboard, select the repository you just created to go to its repository page.
2. Click on the green button called "Code" and copy the HTTPS URL of your repository.
3. Once that is copied, open up Git Bash and type the command "git clone https://github.com/UserName/RepoName/"
4. This will clone your Git Hub repository onto your computer.
5. To move into your repository, type the command "cd RepoName"
6. You have now cloned your repository and can start to work on it within Git Bash.
## Step 4: Creating a New Branch
1. When creating a new branch, you will first have to be on the repository you want to create a branch on.
2. Once in the repository, you can create a new branch using the command "git checkout -b BranchName"
3. This command will create a new branch and allow you to work on seperate stuff without being in the same branch.
## Step 5: Pulling and Pushing from Git Bash
1. When you are working in Git Hub specifically, it won't be saved to your cloned repository on your computer. This is where the pulling command comes into play.
2. When you want to send your edits made on Git Hub to your computer, use the command "git pull origin main" on Git Bash.
3. This will fetch the edits made on Git Hub to Git Bash and the cloned repository.
4. To push edits made on Git Bash to Git Hub, you will use the push command.
5. First make an edit to your README.md file using the nano feature.
6. Once any edit has been made to the README.md file, type "git add README.md" to add the edited file.
7. Once that is done, you will have to commit your changes by using the command "git commit -m 'Description of edit'". The commit will help Git Hub know what edits were made to the file.
8. Finally you can push the edit to github by using the command "git push origin RepoBranchName"
## Step 6: Merge and Merge Conflict
1. When merging branches, this you merge all edits made on the seperate branches to the main branch on your repository.
2. Switch to your main branch by using "git checkout main".
3. Once there, make sure you have the up to date edits on Git Hub by using the pull command.
4. Next you type the command "git merge RepoBranchName". This will merge the specific branch you mention to the main branch.
5. Usually everything will go smooth if you do this, but sometimes a merge conflict will occur.
6. A merge conflict occurs when two branches made the same edit to the same line in a file. This will cause a flag to be raised because it doesn't know what edit to save.
7. To fix this, you will have to go to the file that is flagged and chose what edit to save. Erase the flag markers (<<<<<<< HEAD >>>>>>>) and save the now fixed file.
8. Finally add the file to the main branch "git add ...", make a commit "git commit -m '...'", and finally push the fix to Git Hub (git push origin main).
# Part 2: Glossary of Major Terms Used
1. **Brnach**: A parallel version of a repository that diverges from the main line of development, allowing you to work on features or fixes independently without affecting the primary project codebase.
2. **Clone**: The action of downloading a complete copy of an existing remote repository from a hosting platform like GitHub onto your local machine, preserving its full history and structural tracking.
3. **Commit**: A saved snapshot of staged file modifications stored directly within your local repository's history, acting like a permanent checkpoint marked by a descriptive log message.
4. **Fetch**: A command that downloads new data, branch updates, and commit histories from a remote repository to your local system without merging or modifying your active working files.
5. **Git**: A free, open-source, distributed version control system designed to run locally on your computer to track changes in source code over time.
6. **Git Hub**: A cloud-based web platform that hosts Git repositories online, providing collaboration tools, graphical interfaces, pull requests, and project management capabilities.
7. **Merge**: The process of taking the history and changes from one development branch and combining them directly into another active branch.
8. **Merge Conflict**: A development event that occurs when Git cannot automatically determine the correct code to keep because two separate commits modified the exact same lines of a file, requiring manual developer intervention to resolve.
9. **Push**: The command used to upload your local repository commits directly to a remote hosting platform like GitHub so they can be viewed or shared by others.
10. **Pull**: A single command that fetches data from a remote server and immediately integrates/merges it into your current local working branch to ensure you have the latest updates.
11. **Remote**: The version of your project repository hosted on the internet or a shared network (such as on GitHub) rather than stored locally on your physical machine.
12. **Repository**: The foundational project folder or directory tracked by Git that stores all project files, resource configurations, and the complete chronological history of every adjustment made.
