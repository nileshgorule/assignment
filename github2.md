Push, Commit, Add:

1.What does the "git add" command do in Git?

ans:

adds a new or change files in your working directory to the git staging area.

2.How do you stage changes for a commit in Git?

ans: 
 
As you are working, you may be adding, editing and removing files. But whenever you hit a milestone or finish a part of the work, you should add the files to a Staging Environment.

after adding file it will goes to staging area our file is ready to commit to check that we need to give command 

	-git status

3.What is a Git commit, and how is it different from a push?

ans: 
1.git commit is the record of change.
2.push is upload local repository  content to remote repository.
  
4.How can you create a Git commit with a commit message?

ans:
from the help of below command:

	-git commit -m "some message" 

5.What does "git push" do in Git, and why is it important?

ans:
1.push is upload local repository  content to remote repository.
2.this is useful when you want to share your code with other developers or store it in a remote location for backup purposes.

6.How do you push your local Git commits to a remote repository?

ans:
1.with the help of push command we can psuh local git commit to a remote repository for that we need to give push command.

	-git push origin main

7.Can you explain the difference between "git add" and "git commit"?

ans:

1."git add" : adds new or change files in your working directory to the git staging area.

2."git commit" : it is the record of change.Adding commits keep track of our progress and changes as we work.  

Config:

8.What is the purpose of Git configuration settings?

ans:

1.Git config is a powerful Git command that allows you to customize how Git works and optimize it to fit your workflow.

2. the purpose  of configuring is we need to tell git hub that where and which account we are creating changes or adding files.

9.How do you set your Git username and email globally?

ans :
	git config --global user.name "Your Name"
	git config --global user.email "your.email@example.com"

we can use above command and set username and email globally.


10.What is the difference between local and global Git configurations?

ans:

1.System Git config controls settings for all users and all repositories on your computer.

2.Global Git config controls settings for the currently logged in user and all his repositories.

3.Local Git config controls settings for a specific repository.

4.Global configuration values are applied to a single user and can overwrite system configuration values.

5.Local configuration values apply to a single repository and can override all above and set repository specific options.

11.How can you view your Git configuration settings?

ans:
1.To view your Git configuration settings, you can use the following command in your terminal:

	git config --list

This command will display a comprehensive list of all Git settings, including user information, aliases, core behaviors, and more.

12.Why is it important to configure your Git identity?

ans: 
1.This is because every Git commit uses this information, and it’s immutably baked into the commits you start creating.

2.By setting your identity, you can ensure that your contributions are properly attributed to you and that other users can easily identify who made the changes.

Merge, Pull, Branch:

13.What is a Git branch, and why do we use them?

ans:
1.branch is a new/separate version of the main repository.

2.A branch is a parallel version of a repository. 

3It is contained within the repository, but does not affect the primary or main branch allowing you to work freely without disrupting the "live" version. When you've made the changes you want to make, you can merge your branch back into the main branch to publish your changes.

14.How do you create a new Git branch?

ans:

	git checkout -b<new branch name>

from above command we can create a new git branch.

15.What is the "git merge" command used for in Git?

ans:
1."git merge" command is used for merging to branches.

2.The git merge command in Git is used to integrate changes from one branch into another. 

3.It is typically used to combine changes made on a feature branch with the main branch (usually master).
  
16.How do you merge changes from one branch into another?

ans:
	 git merge<branch name>

using above command we can merge one branch to another.

17.What is a merge conflict, and how can you resolve it?

ans:

1.An,event that takes place when git is unable to automatically resolve differences in code between to commit.

Here are the steps to resolve a merge conflict:

	-Open the conflicted file and make any necessary changes.

	-Use the git add command to stage the new merged content.
	-Create a new commit with the help of the git commit 	command. Git will create a new merge commit to finalize 	the merge.

18.What is the purpose of the "git pull" command in Git?

ans:

used to fetch and dwonload content from a remote repository and immediately update that local repository to match that content.

19.How do you update your local repository with changes from a remote repository using "git pull"?

ans:

	-git pull origin main 

using above command we can update local repository.

20.Can you explain the difference between "git merge" and "git pull"?

ans:
1."git merge" command is used for merging to branches.

2.The git merge command in Git is used to integrate changes from one branch into another. 

3.It is typically used to combine changes made on a feature branch with the main branch (usually master).

4. "git pull" used to fetch and dwonload content from a remote repository and immediately update that local repository to match that content.
 
5.-git pull origin main   using this command we can update local repository.

General Git:

21.What is Git, and what problem does it solve in software development?

ans: 

Git is a popular version control system. It was created by Linus Torvalds in 2005, and has been maintained by Junio Hamano since then.

It is used for:

Tracking code changes
Tracking who made changes
Coding collaboration

22.How do you initialize a Git repository in a directory?

ans:
1.To initialize a Git repository in a directory, navigate to the directory in your terminal and run the command:
	
	 git init


This will create an empty Git repository in the current directory. 

23.How do you check the status of your Git repository?

ans: 
using bewlow command we can check status of your git repository:

	git status

24.What is the purpose of the ".gitignore" file in Git?

ans:
1.The .gitignore file is a text file that instructs Git to ignore certain files or folders in a project. It is usually kept in the project’s root directory.

2.The files or folders listed in .gitignore are intentionally untracked and should be ignored by Git.

3.It is important to note that changes to files that were staged before being added to the .gitignore file will continue to be tracked by Git.

25.How can you view the commit history of a Git repository?

ans: 
1.To view the commit history of a Git repository, you can use the command: 

		git log

2.This command is used to display the commit history of a repository in reverse chronological order, with the most recent commits appearing first.

26.How do you create a new Git repository on a remote hosting service like GitHub or GitLab?

ans:

To create a new Git repository on a remote hosting service like GitHub or GitLab, you need to follow these steps:

1.Create a new repository
	-to create a new repository on GitHub, you can click on 	the “New” button on the main page and then follow the 	prompts to create a new repository.

2.Clone the repository:

	-to your local machine using the "git clone" command.
	- This 	will create a copy of the remote repository on 	your local machine.

3.Add files
	
	-to your local repository using the git add command.
	-This will stage the changes you have made and prepare 	them for committing. 

4.Commit changes

	-to your local repository using the "git commit" command. 	-This will save your changes to your local repository.

5.Push changes

	-to the remote repository using the "git push" command. 	-This will upload your changes to the remote repository.


example:

	-Log in to your GitHub account and click on the “New” 	button.

	-Enter a name for your new repository and select whether 	it should be public or private.

	-Click on the “Create Repository” button.

	-Copy the URL of your new repository.

	-Open up a terminal window and navigate to the directory 	where you want to store your local copy of the repository.

	-Type git clone followed by the URL of your new 	repository.

	-Add files to your local copy of the repository using git 	add.

	-Commit changes using git commit.

	-Push changes to the remote repository using git push.


27.what is the purpose of a Git remote?

ans:

1.A remote in Git is a bookmark for a different repository from which you may wish to pull or push code. 

2.It is a reference to a repository other than the one on your local disk which you can push your changes into (so that other people can see them) or pull from (so that you can get others changes).

28.How can you add a remote repository to your local Git repository?

ans:

1.To add a remote repository to your local Git repository, you can use the command.

	git remote add origin <link/URL>

2.This command takes two arguments: 

the name of the remote and the URL of the remote repository 

29.what is the Git workflow for making changes, committing, and pushing to a remote repository?

ans:

the workflow of git is :

github repo --> clone -->  changes --> add --> commit --> push


30.How do you undo the last Git commit?

ans: 

1.To undo the last commit in Git, you can use the following command:

	git reset HEAD~1

2.This command will remove the last commit from your Git history. The changes made to your files will be preserved, and you can add them again before committing them again.

3.If you want to undo the last commit while preserving the changes made to your files, you can use the following command:

	git reset --soft HEAD~1

This command will move the present branch backward by one commit, effectively undoing your last commit.

4.for many changes 

	git reset <commit hash>

