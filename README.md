# git-learning
Git Learning

This repository was used to learn git commands. Below are the commands that are learnt.

# GIT CONFIGURATION (GLOBAL SETTINGS)
	git config --global user.name "abc xyz"  - This command configure user name at global setting. If there is a space in username then it should be											   between quotes.
	git config --global user.email abc@xyz.com - This command configure user name at global setting. There is no space in user email. That is the reason 			 								  why it is not in quotes.

	git config --global core.editor "code --wait" 
		- This command configure editor. Search "Code" in Visual Studio (command + shift + p) and install it. Go back to terminal and type command "code". 
      It will open visual studio. If you type command "code fileName" then it will open that file

	git config --global -e
		- This command will open your editor. In this case, Visual Studio editor will be opened

	git config --global core.autocrlf xyz - This command is for handling Line Ending.
		- For Mac users, replace xyz value with input
		- For Windows users, replace xyz value with true


# INITIALIZE GIT REPOSITORY
	git init - This command will initialize git repository


# GET THE STATUS
	git status - Gives the status. For example, which files are staged and ready to commit, untracked. Few more details.


# BRANCH
	git branch - Gives the branch

# ADD FILES TO STAGING AREA
	git add file1, file2 - This command will stage file1 and file2 to the Staging Area / Index. You can specify more files with comma separated
	git add . - This command will stage all the files under the current path/ directory to the staging area / Index
	git add -A - This command will stage all the files in the the working directory. In this command, it doesn't matter in which directory or current path 			    you are.


# UNSTAGE FILES FROM STAGING AREA
	git rm --cached <file> - This command will unstage the staged file/files
	git rm -r --cached . - This command will unstage all the staged files


# COMMIT FILES
	git commit -m  "Provide meaningful message for the commit so that others can understand what this commit is related to"
		- This command commit files with meaning message so that other developers can understand it


# DISCARD CHANGES
	git restore <file> - This command is used to discard changes in working directory


# AMEND 
	git commit --amend -m "Provide the message to update". This command amend commit message. The message which was specified in previous commit will be 														updated with the message provided in this command

# COMMIT HISTORY

	git log - This command will provide commit history. Afer you run this command, every commit will have four pieces of information such as commit 			  (Unique Hash value), Author (your username and email that you provided during configuration), Date (timestamp), and Message

	git show <Commit HashValue> - This command will show you what changes went in for a specific commit. You can get the hashvalue after running git log 							   command and get the hash value for whichever you want to see what changes that went in for that specific commit

# DIFFERENCE IN FILES BETWEEN WORKING DIRECTORY AND STAGING AREA

	git diff - This command gives the difference between working directory and Staging area. For example, let's say if we committed one file to staging	           area. Later, we modified the same committed file in the working directory. Now, to see the difference for the same file between 					   working directory and staging area, you need to use this command


# PUSH CHANGES TO GITHUB
  git push -u origin main - This command is used only once when we first time push the code to GitHub. After that, we use git push
  git push - It will push all the committed changes to GitHub
 
