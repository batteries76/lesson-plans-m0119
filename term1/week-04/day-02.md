# Day 02 — Git, Github & Static Website Deployment
## Outcomes
Students to learn how to use git in their terminal (or/and via a gui app such as Github Desktop). Learn about Github and repositories (i.e. Atlassian Bitbucket). Learn how to upload their static website to a server for deployment.

## On successful completion of this unit students will be able to:
- understand Github and create an online git repository 
- version control their projects locally
- put their work to the online repository
- deploy their work online as a static website

## Guided instructions

## Git & Github
- discuss version control
- discuss history of version control
- discuss SSH, ssh-agent and adding ssh keys (security)
- Connecting to GitHub with SSH activity:
```
have students create personal ssh keys for Github.com
```
- discuss git, local .git folder
- discuss online repositories
- discuss & whiteboard and diagram a push and pull to a git repository
- students install git
- demonstrate git initialization with a project ```git init```
- demonstrate creating .gitignore ```touch .gitignore```
- discuss gitignore file, emphasize it's importance
- demonstrate git status ```git status```
- demonstrate adding a file to git ```git add README.md```
- discuss how to affectivly make a git commit 
- demonstrate a commit ```git commit -m "first commit"```
- demonstrate git status ```git status```
- show the log ```git log```
- discuss adding remote repo to local git ```git remote -v```
- add repo to local ```git remote add git@github.com:User/repo.git```
- demo remote again to view changes ```git remote -v```
- *Optional* create and remove a demo remote repo url to git remote
- visit the online repo, discuss and explain Github.com
- push project to Github repo ```git push -u origin master```
- whiteboard and discuss git branches
- create a new branch ```git branch your-branch-name```
- view branches ```git branch```
- switch to the branch ```git checkout your-branch-name```
- view branches again to view changes
- at this time you can swap between master and the branch
- show the local branch tree ```git log --graph --oneline --all```
- add and commit files, then push the branch to Github
- whiteboard & discuss branch merging
- merge branch back into master after some file changes and commits
- view branches again ```git branch```
- discuss collaboration vs forking
- whiteboard discuss pull requests
- have a student clone your project from github ```git clone git@github.com:User/repo.git```
- after making changes via another computer make a pull request ```git pull```
- git activity
```
- get students to form groups of 3/4
- have one student from each group create a project with git
- have them create text/ruby files
- have each in student the group fork and create their own branches
- have each in student the group pull request changes
```

### Netlify/Deployment
Note: use any deployment service you are comfortable with.
- whiteboard & discuss deployment services
- have students sign up for Netlify
- discuss website Netlify, docs
- *Optional* - have students install the Netlify cli (command line interface)
- demonstrate & deploy a static website via cli or drag-n-drop into the website
- *Optional* - deploy to Netlify from github repo
- have students do the same

## Challenges
- [try github](https://try.github.io/levels/1/challenges/1)
- [Git training (Charles O'Farrell)](https://github.com/charleso/git-training)

## Resources
- [Git](https://git-scm.com/)
- [Github](https://github.com/)
- [Add SSH to Github](https://help.github.com/articles/connecting-to-github-with-ssh/)
- [chris beams](https://chris.beams.io/posts/git-commit/)
- [Github for noobs](https://youtu.be/1h9_cB9mPT8)
- [Netlify](https://www.netlify.com/)
- [Netlify cli](https://www.netlify.com/docs/cli/)


