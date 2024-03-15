## Repository:  
- Also known as **repo**  
- It is a central location where the data is stored and managed.  
- There are different types of repos:  
    - **Local** repo: It is a folder which is present in our desktop/PC, where the code is present. Each repo represents a single project.  
    - **Remote** repo: It is hosted on a server or a remote hosting platform which is accessible over a network. The code which is present here, can be collaboarted and shared with others. Some of the remote hosting platforms are GitHub, GitLab, Bitbucket etc..  
- It is used in the context of version control systems like Git, which is a repository that refers to a location where the history and files of a project are stored, along with metadata like commit messages, branches, and tags.
- A git repository is a workspace which tracks and manages the files within a folder.
- It allows to track the changes, collaborate with the others, and can maintain different versions for a project.  

## Tracked:  
- If a file that has been committed atleast once is a tracked file.  
- Git is aware of them and will be monitoring these tracked files.  
- Git tracks the changes that are made to them.  
- Files that have been previously committed to the repository are tracked.  
- After cloning a repository, all files in the repository are initially tracked.  

## Untracked:  
- A newly created file is an untracked file.  
- Git is unaware of them.  
- Files specified in .gitignore are untracked by Git, even if they are existed in the working directory.  

## Staged:  
- Staged files are modified files that have been marked to be included in the next commit.  
- These changes have been added to the staging area.  
- Files can be moved to the staged state using **git add** command.  
- **Staging area**:
    - Also known as index.  
    - It acts as an interface between the working directory and repository.  

## Unstaged:  
- Unstaged files are modified files that have not yet been staged for the next commit.  
- These changes have been made in the working directory but have not been added to the staging area.  

## Flowchart - File Lifecycle:   

   ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/concepts/images/git_status_flowchart.png)  
   