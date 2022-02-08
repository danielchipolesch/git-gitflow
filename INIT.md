![git img](https://www.embarcados.com.br/wp-content/uploads/2015/02/imagem-de-destaque-39-850x510.png)
# How to initialize any project
How to initialize any new project with git e git flow before adding any framework or library.

## Checking git and git flow version

```
$ git --version     // git version 2.33.0.windows.1
$ git flow version  // 1.12.3 (AVH Edition)
```


## Create Project
### Go to repositories path and type on shell:

```
$ mkdir project-name  // It creates a path named "project-name"
$ cd project-name     // This command you enter in that path
```

## Git flow init
### Type:

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
