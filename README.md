# Git and Git-hub setup Guide

### STEP 1 - CREATE A GIT-HUB ACCOUNT
 -First thing to do, you need to create a github account if you have not done. In your account you will save all the repositories that you will be working.

### STEP 2 - INSTALL GIT BASH
- Second thing to do, you need to install git from this link. Make you sure that you install the correct version for your device.
 https://git-scm.com/downloads

### STEP 3 - LOCATE THE WORKING FOLDER ON YOUR LOCAL MACHINE AND GENERATE SSH KEY
- Open Git Bash
- Go to your working folder where you would like to save your project in the local machine and create the new folder:
`mkdir name_of_the_project
cd name_of_the_project`
-Type the following command to generate the SSH key:
`ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`
-Press ENTER in all the steps, leaving empty the gap.

### STEP 4 - FIND AND ADD THE KEY IN YOUR GIT-HUB ACCOUNT
- Open GIT BASH
You should navigate to find the SSH key pair by using:
`cd /c/Users/your_account/.ssh`
List the directory by using:

`ls`
- We could see our SHH key, that it corresponds with the .pub file, so let go to open the file by using:
`cat filename.pub`
-You should see a long line of text in the terminal. Copy the whole text starting with "ssh-rsa".
-Go to your account of Git-Hub and log in.
-Click on your profile picture at the top of the right on the screen and after that click on the option of settings.
-Find the option "SSH and GPG Keys" in the menu on the left of the screen and click on it.
-Click on the option Add a new SSH key.
-Write down a logical name of the Key related to the project, and paste the key.
 -Finally click add SSH key and we will save the public key in our account of Git-Hub
###STEP 5 - CREATE REPOSITORY ON THE COMMAND LINE
-Open GIT BASH
-Go back again in your folder where you will saved your project in the local machine.
-Follow the following commands: Create the file README
-initiate git
`
git init`
Add the file README to the repository

`git add README.md`
Commit the changes with a brief description
`
git commit -m "first commit"`
Change the branch
`
git branch -M main`
Locate repository
`
git remote add origin https://github.com/your_name_account/name_of_repository.git`
Push

`git push -u origin main`

