# Use this as your quick reference guide to Git!

- [Check branch ops instead?](./BRANCH.md)

Here is how:

## To either, initialise a project
- Make a dir where you want to build a project.
- To start/initialise the project use command: <br>
	> git init
- Make a repo using dashboard [Its easy and fast].
- Use the command below to add remote origin: <br>
	> git remote add origin git@something:fooHimanshu/something
- Make sure that you have <b>Generated and Connected the SSH key to github</b>. For ref: <br>
	> https://docs.github.com/en/authentication/connecting-to-github-with-ssh/about-ssh

## OR Clone
- Use the command: <br>
	> git clone gut@something:userName/someRemoteRepo

## Basic git commands
- To check what files has been created, updated or updated but haven't been committed yet.
	> git status

- To add a file to git tracker (Staging)
	> git add <file name>

- To unstage a file:
	> git reset <file name>

- To commit a changes [saves locally]
	> git commit -m "This is the title of the commit" -m "this is the description of the commit"

- To un-commit the last committed file:
	> git reset HEAD~1
	- HEAD is just a pointer to the last commit
	- ~1 means go back to one commit back

- To un-commit a specific commit:
  - Get the hash of the commit by
    > git log

  - Copy the hash and then
    > git reset `hash`

  <b>NB! this won't push changes to remote dir</b>

- <b> To remove commits after a certain commit <i>(rolling back in time)</i> <b>
  > git reset --hard hash

  <b> CAREFUL! OKAY? I AM SURE YOU KNOW WHAT YOU'RE DOING. :)  \\__(0_0)__/</b>

- To push the changes
	> git push origin master <br>

  <b>OR<b> <br>

  	> git push -u origin master
  		- The -u flag makes it obvious that all changes should be pushed to origin master.
  		- This way only ``git push`` could be used in future.

## The local git workflow
![](/static/img/gitLocalWorkFlow.png)
