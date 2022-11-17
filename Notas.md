# GIT
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

## Sections
- [GIT](#git)
  - [Sections](#sections)
  - [Command lines - Local Repository](#command-lines---local-repository)
  - [New Repository GitHub](#new-repository-github)
  - [Push an existing repository from the command line](#push-an-existing-repository-from-the-command-line)
  - [Branch](#branch)
  - [Referencias](#referencias)
## Command lines - Local Repository
- Create a new Git local repository:
    1. **git init**
        El comando git init crea un nuevo repositorio de Git. Puede utilizarse para convertir un proyecto existente y sin versión en un repositorio de Git, o para inicializar un nuevo repositorio vacío.
    2. **git add _fileN or directory_**
        Add file contents to the index
        - **git add .**   add everything inside the directory
        - **-git rm --cached _fileN_**   to unstage from index
    3. **git status**
        return the changes to be commited
    4. **git commit _-m "Comentarios de carga"_**
        Record changes to the repository
        - **git commit --amend** modifica el commit local, usar antes del push, :q cerrar, :wq, :x
        - **git reset HEAD^ --hard** borra el ultimo commit en local
        - **git push origin -f** before reset Head to delete commit on repository
        - **git log**   Shows the commit logs.
- Restore data
    1. **git diff**  Show changes between commits, commit and working tree, etc
    2. **git checkout _fileN_** Restore working tree files, also git checkout switch branches
        - _git chechout ._ restore everything from inside the directory that has changes for the last commit.
## New Repository GitHub
How to create a new repository on github
![Create a new repository](images\New_repository_github01.png)

## Push an existing repository from the command line
-
    1. **git remote add origin https://github.com/Max-Madin/My-GitHub-Demo.git**
        - **git push origin -f** force the changes to repository, delete ultimate commit**
    - **git branch -M master**
    2. **git push -u origin master**
## Branch
- Create a new branch local
    - **git branch _name of the branch_ _optinal CommitShar_** 
        creates a new branch, commitshar = 10870982cfdb5570e95787ec3fb071cb5e43ee4c last of url commit and is the father of the new branch, default ultimate commit of master
        - **git branch** list the name of the branches        
        - **git branch -d _branch-name_** Delete a local branch, if change -d to -D forces deleting of branch commits.
        - **git checkout _name of the branch_** Switch branches
        - **git checkout -b _NewNameBranch_ _CommitShar_** create and switch to a new branch
- Mix branches
    1. position on master branch _git checkout master_
    2. **git merge**
- URL of remote branch
  - **git remote show** regresa => _origin_ el resultado se agrega al final
  - **git remote show _origin_**
## Referencias
<https://www.atlassian.com/es/git>
<https://git-scm.com/book/en/v2>
<https://training.github.com/downloads/github-git-cheat-sheet.pdf>