##Mastering Git
##Part 3: Navigating Git-Unraveling Commits and Branches

![Alt text](<images/Mastering git 3.drawio.png>)

## Introduction:
Welcome back to our Git journey! Previously we were unveiling the Mysteries of Git Objects and Committing Changes. In Part 3, we're going to dive into the exciting world of checking out commits and branches. This is where Git's time-traveling abilities truly shine. Let's get started!


### Checking Out Commits and Branches

To embark on this adventure, we'll be using the trusty `git log` command to help us navigate Git's vast landscape.

**Note:** Keep an eye on the `HEAD` – it's like your GPS in Git, showing you where you currently are.

## Moving to the 'First Commit' Using 'Git Checkout'

First, let's journey back in time to our project's humble beginnings – the 'First Commit.'

#### Step 1: Checkout Commit

To do this, we'll need the commit's unique identifier, also known as the SHA1 hash. You can find this information using the `git log` command.

```bash
git checkout [hash]
```

You can use the full hash or a shortened version – Git is smart enough to figure it out.

Example:

```bash
git checkout b0cecd5e7fa3a0bc9102582fd66766c33287ed05

# Or use the short version
git checkout b0cecd5
```

As you execute this command, notice how your terminal location changes, indicating that you've just traveled back in time.

```bash
~/local-repo ((b0cecd5...))
```

#### Step 2: Listing Files in the 'First Commit'

Now that we're in the past, let's see what our project looked like at its inception.

```bash
ls
```

You'll likely find just one file – a testament to the project's early days.

## Moving to the 'Main' Branch Using 'Git Checkout'

Next, we'll return to the present and switch to the 'Main' branch.

#### Step 1: Checkout 'Main' Branch

To do this, we'll use the `git checkout` command with the branch name.

```bash
git checkout main
```

Again, your terminal location will reflect this move.

```bash
~/local-repo (main)
```

#### Step 2: Listing Files in the 'Main' Branch

Now that we're back in the 'Main' branch, list the files in the directory to see how the project has evolved.

```bash
ls
```

You should now see both `devops.txt` and `providers.txt` files, a testament to the progress we've made.

With these newfound skills, we're ready to tackle Git merging and explore even more of what this powerful tool can do. Stay curious and keep coding! 🚀🌟 #GitMastery #TimeTravelWithGit #BranchingOut #VersionControl #LearnGit
