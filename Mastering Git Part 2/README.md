## **Mastering Git:**
## **Part 2 : Unveiling the Mysteries of Git Objects and Committing Changes**

![Alt text](<images/Mastering git 2.drawio.png>)

**Introduction:**
In our last episod of Mastering Git Part 1 we learned about creating a local repo. let's continue our journey through Git as we're now delving into the fascinating realm of Git objects and the crucial process of committing changes. These are the building blocks of version control, and understanding them is key to becoming a Git maestro. So, let's roll up our sleeves and dive in!


### Reading Git Objects

We begin with the thrilling task of decoding Git objects. These objects store everything in Git, from your files to commit history.

#### Step 1: Listing Created Objects

```bash
ls .git/objects
```

This command reveals a treasure trove of directories and files that represent Git objects. Each object possesses a unique hash.

#### Listing Object Hash

```bash
ls .git/objects/b0
```

Explore one of these directories to uncover the hash of a specific Git object. These hashes serve as fingerprints for Git objects.

#### Listing Object Type (git cat-file -t)

```bash
git cat-file -t b0cecd5e7fa3a0bc9102582fd66766c33287ed05
```

Execute this command to identify the type of Git object associated with the provided hash. Git objects can be blobs, trees, commits, and more.

#### Listing Object Content (git cat-file -p)

```bash
git cat-file -p b0cecd5e7fa3a0bc9102582fd66766c33287ed05
```

This command unveils the actual content stored within the specified Git object. It's like peering into the heart of Git.

### Creating, Adding, and Committing a Second File in the local-repo Directory

Now, let's transition from dissecting Git objects to making changes within our Git repository.

#### Step 1: Creating a Second File: providers.txt

```bash
echo 'AWS, AZURE, GCP, and OCI' > providers.txt
ls
cat providers.txt
```

In this step, we've crafted a new file, 'providers.txt,' within the 'local-repo' directory.

#### Step 2: Checking Git's Mood (Status)

```bash
git status
```

Before proceeding, let's ask Git how it feels about our changes. At this point, 'providers.txt' is an untracked file.

#### Step 3: Adding Files to the Stage Area

```bash
git add .
```

To prepare our changes for the grand commit, we've added all files, although in this case, it's just 'providers.txt,' to the staging area.

#### Step 4: Checking Git's New Mood (Status)

```bash
git status
```

Now, our changes are staged and ready for their moment of glory, the commit. This step is vital for documenting your work.

#### Step 5: Committing Changes

```bash
git commit -m 'Second DevOps Cloud Bootcamp commit'
```

Finally, we commit our changes with a message, giving context to the changes. This is the hallmark of organized version control.

### Commits History

To wrap up, let's revisit our commit history, the chronicles of our project's evolution.

#### Step 1: Checking Git's Memory (Commit History)

```bash
git log
git log --oneline
```

This command lets us travel back in time, exploring all our commits and their concise summaries.

Stay tuned for more Git adventures in Mastering Git Part 3. Understanding Git's inner workings is like wielding a developer's superpower. Happy coding! 🚀📜 #DevOps #GitMastery #CommitChanges #VersionControl #LearnGit