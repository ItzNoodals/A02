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
## Step 4: Pulling and Pushing from Git Bash
1. When you are working in Git Hub specifically, it won't be saved to your cloned repository on your computer. This is where the pulling command comes into play.
2. When you want to send your edits made on Git Hub to your computer, use the command "git push origin main" on Git Bash.
3. This will pull on edits made on Git Hub to Git Bash and the cloned repository.
4. To push edits made on Git Bash to Git Hub, you will use the push command.
5. First make an edit to your README.md file using the nano feature.
6. Once any edit has been made to the README.md file, type "git add README.md" to add the edited file.
7. Once that is done, you will have to commit your changes by using the command "git commit -m 'Description of edit'". The commit will help Git Hub know what edits were made to the file.
8. Finally you can push the edit to github by using the command "git push origin RepoBranchName"
