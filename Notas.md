# GIT
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

## Sections
- [GIT](#git)
  - [Sections](#sections)
  - [Command lines - Local Repository](#command-lines---local-repository)
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
        - **git log**   Shows the commit logs.
- Restore data
    1. **git diff**  Show changes between commits, commit and working tree, etc
    2. **git checkout _fileN_** Restore working tree files, also git checkout switch branches
        - _git chechout ._ restore everything from inside the directory that has changes for the last commit.

## Referencias
<https://www.atlassian.com/es/git>
<https://git-scm.com/book/en/v2>
<https://training.github.com/downloads/github-git-cheat-sheet.pdf>