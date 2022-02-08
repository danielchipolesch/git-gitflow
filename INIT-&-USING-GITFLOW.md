# STARTING ANY NEW PROJECT
<h2 align="justify"> Starting any new project with git-flow before adding any file, path, framework or library.</h2>

- [x] Basic commands
- [ ] What happens after creating new release ?

## Checking Git and Git Flow version

```
$ git --version     // git version 2.33.0.windows.1
$ git flow version  // 1.12.3 (AVH Edition)
```

## Creating Project
### Go to repositories path and type on shell:

```
$ mkdir project-name  // It creates "project-name" path 
$ cd project-name     // Enter in the path
```

## Using Git Flow Init

```
$ git flow init

No branches exist yet. Base branches must be created now.
Branch name for production releases: [master]
Branch name for "next release" development: [develop]

How to name your supporting branch prefixes?
Feature branches? [feature/]
Bugfix branches? [bugfix/]
Release branches? [release/]
Hotfix branches? [hotfix/]
Support branches? [support/]
Version tag prefix? []
Hooks and filters directory? [D:/Documentos/nodeprojects/project-name/.git/hooks]
```

## Starting a new Feature Branch
```
$ git flow feature start feature_branch_name
```
### It returns this message
```
Switched to a new branch 'feature/feature_branch_name'

Summary of actions:
- A new branch 'feature/feature_branch_name' was created, based on 'develop'
- You are now on branch 'feature/feature_branch_name'

Now, start committing on your feature. When done, use:

     git flow feature finish feature_branch_name
```

### Commit new changes normally
```
$ git add .
$ git commit -m "feat: commit message"
```

## Finishing Previous Branch
```
$ git flow feature finish feature_branch_name
```
### It returns this message
```
Switched to branch 'develop'
Updating 9244e64..535e909
Fast-forward
 Filename.extension | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Filename.extension
Deleted branch feature/feature_branch_name (was 535e909).

Summary of actions:
- The feature branch 'feature/feature_branch_name' was merged into 'develop'
- Feature branch 'feature/feature_branch_name' has been locally deleted
- You are now on branch 'develop'
```

> Repeat this commands above how many times you need

<h6 align="justify"> Once the develop branch has enough resources for a release, you fork a release branch from the develop branch. Creating this branch starts the next release cycle, so no new features can be added after this point — only security updates, documentation generation, and other release-related tasks should go in this branch. When ready to be released, the release branch is merged into the main branch and marked with the version number. It should also be merged back into the develop branch, which may have progressed since the release started. Using the dedicated release staging branch makes it possible for one team to improve the current release while another team continues to work on features for the next release. It also creates well-defined development phases (for example, it's easy to say "This week we're getting ready for version 4.0" and actually see what the repository structure looks like). Building release branches is another simple branching operation. Like feature branches, release branches are based on the development branch. A new release branch can be created using the following methods.</h6>

## Creating a New Release
```
$ git flow release start 0.1.0
```
### It returns the message below
```
Switched to a new branch 'release/0.1.0'
```
