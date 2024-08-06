Basic Git Workflow
git init
Now that we have started working on the screenplay, let’s turn the sorcerers-code directory into a Git project. We do this with:

git init

The word init means initialize. The command sets up all the tools Git needs to begin tracking changes made to the project.

2. line
git status
As you write the screenplay, you will be changing the contents of the working directory. You can check the status of those changes with:

git status

3. line
   git add
In order for Git to start tracking scene-1.txt, the file needs to be added to the staging area.

We can add a file to the staging area with:

git add filename

The word filename here refers to the name of the file you are editing, such as scene-1.txt.

git diff
Good work! Now you know how to add a file to the staging area.

Imagine that we type another line in scene-1.txt. Since the file is tracked, we can check the differences between the working directory and the staging area with:

git diff filename

Here, filename is the actual name of the file. If the name of my file was changes.txt the command would be

git diff changes.txt

Instructions
Checkpoint 1 Passed
1.
In the code editor, add this text to scene-1.txt:

Dumblediff: I should've known you would be here, Professor McGonagit.

Click Run.

Checkpoint 2 Passed
2.
From the terminal, use the new command to check the difference between the working directory and the staging area.

Notice the output:

“Harry Programmer and the Sorcerer’s Code: Scene 1” is in the staging area, as indicated in white.
Changes to the file are marked with a + and are indicated in green.

git commit
A commit is the last step in our Git workflow. A commit permanently stores changes from the staging area inside the repository.

git commit is the command we’ll do next. However, one more bit of code is needed for a commit: the option -m followed by a message. Here’s an example:

git commit -m "Complete first line of dialogue"

Standard Conventions for Commit Messages:

Must be in quotation marks
Written in the present tense
Should be brief (50 characters or less) when using -m


git log
Often with Git, you’ll need to refer back to an earlier version of a project. Commits are stored chronologically in the repository and can be viewed with:

git log

Instructions
Checkpoint 1 Passed
1.
From the terminal, log a list of your commits.

In the output, notice:

A 40-character code, called a SHA, that uniquely identifies the commit. This appears in orange text.
The commit author (you!)
The date and time of the commit
The commit message



