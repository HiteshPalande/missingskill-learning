

















# 												GIT

























---





## About GIT 



Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

With GIT  we can control the version of our system. Git basically tracks the changes in the project files, because of this we can work on those files among multiple people since all changes are controlled ny GIT.

Git tracks every file. And, since we keep all the history of our files, we can roll back a specific part of your project.  



#### Different Type of VCS

Following are the different version control software(VCS) used by companies.

- GitHub
- GitLab
- AWS(Amazon Web Services)
- Beanstalk
- Cloud Source by Google

GIT is one of the most popular VCS available in market. following are the advantages of GIT.



#### Advantages of Git

- Git is simple to use
- Git records everything, it has recording system where it record everything & we can also collaborate
- Provides the best performance when it comes to version control system. Committing, branching,merging all are optimized for a better performance than other system
- Git is an Open Source so it has a huge community which helps it to make itself more powerful.





---





## Branching and Merging in GIT

- Anything in the `master` branch is deployable 
- To work on something new, we need to create a branch from`master` and we can give a name to it
- we can commit to that branch locally and regularly push our work to the same named branch on the remote server
- When we need  data from other branch, or if we think the branch is ready for merging, we can do a pull request
- Once it is merged and pushed to `master`, we can  deploy 



Lets take an example of Branching with the help of following image



![GitFlow](https://github.com/HiteshPalande/missingskill-learning/blob/main/Images/GitFlow.jpg)



We can an example of Educational System where everyone has to take a basic education that is from 1st to 10th standard. Here consider School as a `master` branch, similarly in GIT we have `master` as a main branch .

After 10th we have privilage to choose any branch like Science, Commerce, Arts, etc. and further we can select another educational from Higher College. Similarly in GIT we can create other branch from `master` branch and further we can have other branches also.





----





## Most used commands in GIT

| Sr. No | Commands                     | Description                                                  |
| :----: | ---------------------------- | ------------------------------------------------------------ |
|   1    | git init                     | Creates new/empty repository                                 |
|   2    | git add [fileName]           | To add files to the staging area for committing              |
|   3    | git add                      | To add the all files at once to the staging area for committing |
|   4    | git commit -m"[message]"     | To commit the changes of the files added previoyusly         |
|   5    | git log                      | It shows history of all the previous commits                 |
|   6    | git diff                     | Shows the difference which are updated                       |
|   7    | git show [commitId]          | Shows changed made in perticular file, used for tracking purpose |
|   8    | git status                   | Shows the current status of git tree                         |
|   9    | git branch                   | Shows all the branches and points to the branch which is been used by user by a "*" sign |
|   10   | git branch [branchName]      | To create new branch                                         |
|   11   | git checkout [branchName]    | To switch from one branch to another                         |
|   12   | git checkout [fileName]      | To revert new changes done in the file                       |
|   13   | git checkout [fileName]      | If the given file is not present in local system then with this command we can recover the file |
|   14   | git push origin [branchName] | To push all the changes from lacal repository to remote repository |
|   15   | git pull origin [repository] | To pull all the changes from remote repository to the local machine |
|   16   | git merge                    | To merges the files from one branch to another branch        |
|   16   | git stash                    | `To create a temporary copy of the files/data which can be used later |
|   17   | git clone                    | To clone remote repository to the local machine              |
|   18   | git reset HEAD [filename]    | To remove file from added state                              |
|   19   | git stash                    | It creates temporary copy of a file which can be used later in another location |
|   20   | git stash pop                | we can recover the recent stashed file which is copied to another location by git stash command within the same branch by using this files |
|   21   | git stash list               | It shows list of all stashed files                           |





---





