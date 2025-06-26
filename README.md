# 16/06/2025 Initial Setup

Let's get this project started! Follow the guide below to set up your Git environment.
Once the project specs are released, I'll update this README with steps to set up our project environment.

## Step 1: Create a GitHub Account
If you've never used GitHub before, the first step is to create your account here: https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github 
Once you've created and verified your account, it may be a good idea to set-up 2FA for better security, but you can do this anytime you prefer.
**Send me your Github username so that I can add you as a collaborator**

## Step 2: Create an SSH Key in your local machine
I believe most of us here use Mac, so follow along to create your SSH key that you will need to contribute to this repository.
1. Open up a terminal.
2. Generate an SSH key with this command. Replace the email in quotes with the email you signed up to GitHub with. Feel free to keep pressing Enter until the key is generated. `ssh-keygen -t ed25519 -C "your_email@example.com"`
3. Start the SSH agent: `eval "$(ssh-agent -s)"`
4. Add the key to your agent: `ssh-add ~/.ssh/id_ed25519`
5. Copy the SSH key: `cat ~/.ssh/id_ed25519.pub`
6. Navigate to `Settings > SSH and GPG keys > New SSH key`
7. Paste the key there and set the expiration to something reasonable. I would do 3 months / 90 days so that you have access until the end of the course.

## Step 3: Clone the repository to your local machine
1. Create a folder and navigate to it. Learn how to do this by reading this guide: https://gist.github.com/bradtraversy/cc180de0edee05075a6139e42d5f28ce, specifically the 'File System Navigation' section. If you are too lazy and don't care where your folder is, follow Steps 2-4
2. `cd ~`
3. `mkdir Lazy9517Project`
4. `cd Lazy9517Project`
5. Now that we have a directory and have navigated into it, let's clone my repository. `git clone git@github.com:huang-jiaming/comp9517project.git`
6. Jump into the directory. Congratulations, you now have access to the project! `cd comp9517project`
7. For sanity, run this command: `git pull` and make sure it says `Already up to date`.

## Create a branch to work on and push changes
When you want to contribute to the project, create a branch first. Any changes you make will be unique to that branch and will have no effect on the core project code. When you are ready to submit your code, create a Pull Request and an Approver will review it before merging it with the main branch.
1. Create a new branch. You can name it whatever you want. `git checkout -b new_branch`
2. Make your modifications.
3. Check your files changed: `git status`
4. Add the files you'd like from the list of files changed: `git add your_file_changed`
5. Alternatively, if you've changed multiple files and you want to add them all: `git add .`
6. Commit your changes with a helpful message. Remember to commit regularly: `git commit -m "your message"`
7. Push your changes for the first time: `git push --set-upstream origin new_branch`
8. Pushing your changes from that branch in the future: `git push`

## Creating a Pull Request
Now that you've done the work and pushed your changes to your branch, you can create a Pull Request. This is the only way your work will be reflected and contribution recorded.
1. Navigate to `https://github.com/huang-jiaming/comp9517project/compare`
2. Change the `compare: main` tab to your branch. It will say `compare: new_branch`
3. If you've properly pushed your changes, there will be a big green button that says `Create pull request`
4. Fill in the Title and Description. Be descriptive and clear.
5. On the right, there is a tab called `Reviewers`. Assign someone with approval permissions to review your code.

## While you wait
In the meantime, you can do whatever you want with your branch, or new branches! New changes will be reflected when you open your next Pull Request. Congratulations on your first contribution to the project!

## TO DO
Thanks for reading to the end of the README. To practice this, and to make sure everyone understands the process, I want you to follow these steps: set-up your GitHub account, set-up your environment, create a new branch, write some dummy code, push, and create a pull request. Follow the steps below on how to create some dummy code once you've created your new branch.
1. Run `git pull`. Do this every time you are about to work on the project, in case new changes have been made. If there are merge conflicts, just message me and we can sort them out together.
2. Create a file and modify it in vim: `vi test.txt`
3. Press `i`. You should see `INSERT` appear on the bottom left of your terminal.
4. Type your name.
5. Press `esc`. This will exit insert mode.
6. Type `:x` and press `Enter`. This will write and save your work, and you should be back in your directory.
