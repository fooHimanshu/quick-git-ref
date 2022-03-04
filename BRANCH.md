# A quick reference guide to Git Branches!

- [Check the basic commands instead?](./README.md)

## Basic branch ops:

- To create a branch. <br>
  > git checkout -b branch feature-xyz <br>
   - -b is to create a Branch.
   - could be read as create and checkout the Branch

   ![](/static/img/gitBranchCreated.png)


- To sync your branch with master:
  - Checkout the master branch to have the changes to your local master.
    > git checkout master

  - Merge the local master to your local Branch.
    > git checkout feature-xyz

    > git merge master

    <b>NB! if there are merge conflict , use an editor to resolve</b>

    ![](/static/img/mergeIssueSolve.gif)

  - keep working until ready to commit and push.

    ![](/static/img/branchesMerged.png)

- To delete a branch:
  > git branch -d feature-xyz
