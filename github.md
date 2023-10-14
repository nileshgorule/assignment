1.What is GitHub?
ans:
1.Git is not the same as GitHub.
2.GitHub makes tools that use Git.
3.GitHub is the largest host of source code in the world, and has been owned by Microsoft since 2018.
4.A GitHub repository can be used to store a development project. It can contain folders and any type of files(HTML, CSS, JavaScript, Documents, Data, Images). A GitHub repository should also include a licence file and a READMEfile about the project. 

2.How do you create a GitHub account?
ans:
step 1: first wew need to dwonload git software and install it our computer.

step 2:  after install we need to configure git with your name and email address. for that  go to  the command prompt on your pc or laptop. replace "your name" and "email address" with your actual name and email.

syntax :
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com

step 3:
example:  
git config --global user.name nileshgourle
git config --global user.email nileshgorule8730@gmail.com

step 4 : after configuring we need  verify our account for that we need to  type below commands.

git config --global user.name
git config --global user.email 

thats'it!

3.What is a repository in GitHub?
ans:
1.repository contain a collection of files of various different versions of a Project. These files are imported from the repository into the local server of the user for further updations and modifications in the content of the file. 

4.How can you create a new repository on GitHub?
ans :
1. on to  github.com go to repository and then click on NEW

2. type the repository name the give some description and after that we can set public or private  if you want readme file  you can  keep it and the create repository.

5.What is a README.md file, and why is it important in a GitHub repository?

ans :
1.README.md file is the guide that gives other developers a detailed description about  project.

2. it contains markdwon formatted text that explains the project basics and point you int the right direction.

3. it important because  file communicates  some importanat information about projectn such as how to install and run it.

4.  in simple words we are explainning our project for the help of readme.md file.

6.How do you add files to a GitHub repository?

ans:
1. go to terminal. 
2. with the following command we can add the files:

	- git add <-file name->
3. then need to commit 
	- git commit -m <some message>
4.once commit done we need to set the branch for that 
	- git branch -m main
 after that we need to set the remote for that 

5.	- git remote add origin <repository link>
 
6.  if you want see out file in our github we need to use push command
	- git push origin main

7.How can you commit changes to a repository in GitHub?

ans :
1. with the help of commit cammand we can commit changes on repository in github.

	- git commit -m <some message>
it is the record of change.

8.What is a pull request, and how do you create one?

ans: 
1.it lets you tell others about changes you've pushed to branch  in a repository on github.

2. to create pull request :
	- click on compare and pull request 
	- and  add new feature
	- create pull request 
	- click  merge pull request.
	- confirm merge.
it will show you message that your pull request successfully merge and closed.
 
9.What is a fork in GitHub?

ans: 

1.A fork is new repository that shares code ans visibility setting with the original "upstream" repository.
2. fork is rough copy.

10. How do you clone a repository to your local machine?

ans: 
1. clone a repository on our local machine we need to go github then go to the project in that <code button> is available we need to click the  go to the  HTTPS and copy the link.

2. then go to  terminal and type command
	-git clone < paste link >

11.How do you push changes from your local machine to a GitHub repository?

ans : 
1. to upload the local repository content to a remote repository use  push command.

	- git push origin main

12.What is a branch in GitHub, and why would you use it?

ans: 
1. Develop features, fix bugs, or safely experiment with new ideas in a contained area of your repository.

2.Isolate your development work from other branches in the repository.

3.Work on different parts of a project without impacting the main branch.

4.Switch between branches and work on different projects without them interfering with each other.

5.Create a separate branch to do your work in (and then later submit that branch for review before it’s merged into the main branch) to avoid pushing buggy code to the production environment.

13. How can you merge a branch into the main/master branch?

ans:
1. with the help of merge command we can merge the  branch to the main branch

	- git merge <branch name>
 
with the help of pull request we can merge the branches.

14.What is the purpose of the "Issues" tab in a GitHub repository?

ans: 
1.The Issues tab in a GitHub repository is a bug tracker for the project. 
2.It is a place where users can report bugs, ask questions, request features, and discuss enhancements of the project.

3.It is also a great place to keep track of tasks and progress of the project 

15.How do you close an issue on GitHub?

ans:

You can close an issue through the GitHub web interface when you're viewing the issue. The "Close Issue" button is to the left of the "comment" button under the comment box. I believe you need to be a collaborator on a repo to close an issue.
















