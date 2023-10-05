## **Mastering Git**

## **PART 1: Creating Repositories and Managing Changes**

![Alt text](<images/Mastering git.drawio.png>)
Introduction:
In the world of DevOps and version control, Git stands as an indispensable tool. Whether you're a seasoned developer or just starting your journey, understanding Git's fundamentals is crucial. In this post, I'll explore the essential steps of creating a new Git repository and managing changes within it. This is a 4 part series of my journey in to becoming a version control expert.

## Creating a New Git Repository: local-repo

Let's kick things off by creating a fresh Git repository from scratch. Follow these steps:

### Step 1: Create a New Directory

Begin by creating a new directory where your Git repository will reside:

```bash
mkdir local-repo
```

### Step 2: Access the New Directory

Navigate into the newly created directory:

```bash
cd local-repo
ls
```

### Step 3: Initializing a Git Repository

Now, initialize a Git repository within this directory:

```bash
git init
```

### Step 4: Listing Hidden Files/Folders

Git keeps some of its essential components hidden. You can reveal them by listing hidden files and folders:

```bash
ls
ls -a
```

### Step 5: Renaming a Branch

By default, Git names its initial branch 'master.' If you prefer to use 'main' instead, you can rename it like so:

```bash
git branch -m main
```

# Adding Changes to the Staging Area

Once you've set up your Git repository, it's time to add changes to the staging area before committing them.

### Step 1: Create a File

First, let's create a file called 'devops.txt' inside the 'local-repo' folder:

```bash
echo 'This is how I became a Devops pro' > devops.txt
ls
cat devops.txt
```

### Step 2: Checking Git Objects

At this stage, it's worth taking a quick look at the Git objects. They will change once the commit process occurs:

```bash
ls .git/objects
```

### Step 3: Checking the Status of Git

To understand what's happening with your changes, use the following command:

```bash
git status
```

**Note:** Untracked files are not being monitored by Git. Currently, the file 'devops.txt' is located only in the Working Directory.

### Step 4: Adding Files to the Stage

To prepare your changes for committing, add the 'devops.txt' file to the staging area:

```bash
git add devops.txt
```

### Step 5: Checking the Updated Status

Confirm that your changes have been added to the staging area by running:

```bash
git status
```

**Note:** Your changes are now staged, awaiting confirmation through a commit.

# Setting Up Author Name and Email

Before you proceed with the commit, it's essential to configure your author information. Replace `<your name/user>` and `<your email>` with your actual name and email address.

```bash
git config --global user.name <your name/user>
git config --global user.email <your email>
```

## Checking Author Name and Email

To ensure your author information is correctly set, use the following command:

```bash
git config --list
```

## Conclusion

Congratulations! You've successfully created a new Git repository and learned how to manage changes by adding them to the staging area. These are foundational Git skills that will serve you well in your DevOps and coding endeavors.

Stay tuned for more Git insights and advanced techniques. Happy coding! 🚀🔍 #DevOps #VersionControl #GitEssentials #CodeInGit #DevOpsJourney #LearnGit