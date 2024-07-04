# PLPBasicGitAssignment
name: MICHAEL KATANA
DATE: JULY 4TH- 2024

Hands-On Assignment: Basic Git And GitHub Workflow
# creating, initializing and commiting files to GitHub account.
## task 1: repository set up
To create a github repository follow the following steps:
    (1) go to https://github.com and log in to your github account or create one.
    (2) click on profile icon, navigate to your repository and click "new"
    (3) input the repository name, in my case "PLPBasicGitAssignment" and add the README.md file and click "Create repository" at the bottom of the page.
    (4) your newly created repo should now show up under repository section.
image on creating a repository:
![creating a repo](<repo_image_1.png>)

## task 2: Local Setup: folder set up
    STEPS:
    (1) Click the windows button and type 'git bash' and run it as an administrator.
    (2) Naviaget to the drive and folder you want to create the "PLPBasicGitAssignment" folder by using the command 'cd drive name'
    (3) create the folder using: 'mkdir folder name'
    (4) Navigate into the created folder, again type: 'cd folder_name'
In my case , to create the folder, I did as in the image below:
![create a local folder](<folder_creation_1.png>)

## task 3: Initializing git on local folder.
    STEP:
    (1) First, navigated to the folder 'PLPBasicGitAssignment' using a commandline or git bash as in my case.
    (2) Type 'git init'
    (3) As my remote branch was main and my local branch was master,
    I had to change my local branch to main to:
    I type: 'git branch -m master main'.
    (4) I then connected my local repo to the remote one on git hub, to do this I typed: 'git remote add origin https://github.com/mickey-gk/PLPBasicGitAssignment.git'

## task 4: Making Changes, Create a File: 
To create the hello.txt file:
    (1) in git bash, I typed: 'touch hello.txt' and the text file was generated.
    (2) to write on the file I typed: 'echo "message to be written" > hello.txt'.

## Commiting changes, staging the fill.
To stage the file, I did the following in git bash:
    (1) git add . to add the hello.txt file and the images.
    (2) git commit -m "commiting a hello.txt file to github".

## Pushing the work to github:
Due to some challenges, I could not push my file directly to github as the local repository was behind the remote repository. This I had to first fetch and create a pull request in order to update the local repo.
    (1) git fetch origin
    (2) git pull origin main --allow-unrelated-histories
    (3) git push -u origin main
By using the above steps, I was able to connect and ush to my remote repository.
![image of pushing to repo](<pushing_to_github.png>)

## verification on github:
I could see my uploaded work when i navigated to my github repository.
Both images, hello.txt file and README.md file were present.