## **MASTERING GIT: **
## Part 4 : Navigating GitHub

![Alt text](<images/Mastering git 4.drawio.png>)
Introduction:
In our ongoing Mastering Git journey, we've covered a lot of ground – from basic commands to branching and history navigation. Now, it's time to take a giant leap forward and explore the exciting world of GitHub. Get ready for some hands-on action in Part 4!

## Hands-on: Git Tasks 

### Pre-requisites

Before we dive into the Git operations, there's a small pre-requisite: you need a GitHub account. If you don't have one, fret not – creating an account is a breeze. Just follow this link: [Signing up for a new GitHub account](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account), and you'll be all set.

Now, let's roll up our sleeves and perform some Git operations, including pushing our code to GitHub!

### Step 1: Create a Private Remote Repository on GitHub

Our first step is to create a private remote repository on GitHub. This repository will serve as the cloud-based home for our project.

### Step 2: Create a Folder `simple-website-repo-poc1`

Next, let's organize our local workspace by creating a folder named `simple-website-repo-poc1`.

### Step 3: Run Git Commands to Create a Local Repository

Now, it's time to initialize our local repository. We'll follow the GitHub Quickstart guide to get things set up just right.

### Step 4: Create File `index.html` and Preview It on AWS Cloud9

To make things interesting, we'll create an `index.html` file for a simple website. We'll then use AWS Cloud9 to preview our creation.

### Step 5: Add This File to Staging and Commit

With our `index.html` file ready, let's add it to the staging area and make our first commit.

```bash
git add .
git commit -m "1st commit"
```

### Step 6: Create a Personal Access Token

To securely authenticate with GitHub, we'll create a personal access token – a crucial step in connecting our local repository to the remote one on GitHub.

### Step 7: Push to Remote Repository

The moment of truth! We'll use the `git push` command to send our local code to the GitHub repository.

```bash
git push -u origin main
```

### Step 8: Explore GitHub Features

Now that our code is safely on GitHub, it's time to explore the platform's powerful features. Dive into the world of issues, pull requests, and collaboration.

Congratulations, we've successfully pushed your code to GitHub! 🎉

Conclusion:
With this hands-on experience, we've taken a significant step in your Git journey. GitHub is a powerful tool for collaboration and version control. Stay curious, keep coding, and explore the vast possibilities that Git and GitHub offer! 🚀🌟 #GitHubMastery #GitPush #VersionControl #GitHubFeatures #LearnGit