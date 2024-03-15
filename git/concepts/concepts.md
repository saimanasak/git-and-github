# Concepts:  

<a name="top"></a>
- [ Repository ](#repository)  
- [ Tracked ](#tracked)  
- [ Untracked ](#untracked)  
- [ Staged ](#staged)  
- [ Unstaged ](#unstaged)  
- [ Flowchart ](#flowchart---file-lifecycle)  
- [ Working Tree ](#working-tree)  

<a name="repo"></a>
## Repository:  
- Also known as **repo**  
- It is a central location where the data is stored and managed.  
- There are different types of repos:  
    - **Local** repo: It is a folder which is present in our desktop/PC, where the code is present. Each repo represents a single project.  
    - **Remote** repo: It is hosted on a server or a remote hosting platform which is accessible over a network. The code which is present here, can be collaboarted and shared with others. Some of the remote hosting platforms are GitHub, GitLab, Bitbucket etc..  
- It is used in the context of version control systems like Git, which is a repository that refers to a location where the history and files of a project are stored, along with metadata like commit messages, branches, and tags.
- A git repository is a workspace which tracks and manages the files within a folder.
- It allows to track the changes, collaborate with the others, and can maintain different versions for a project.  

<a name="tracked"></a>
## Tracked:  
- If a file that has been committed atleast once is a tracked file.  
- Git is aware of them and will be monitoring these tracked files.  
- Git tracks the changes that are made to them.  
- Files that have been previously committed to the repository are tracked.  
- After cloning a repository, all files in the repository are initially tracked.  

<a name="untracked"></a>
## Untracked:  
- A newly created file is an untracked file.  
- Git is unaware of them.  
- Files specified in .gitignore are untracked by Git, even if they are existed in the working directory.  

<a name="staged"></a>
## Staged:  
- Staged files are modified files that have been marked to be included in the next commit.  
- These changes have been added to the staging area.  
- Files can be moved to the staged state using **git add** command.  
- **Staging area**:
    - Also known as index.  
    - It acts as an interface between the working directory and repository.  

<a name="unstaged"></a>
## Unstaged:  
- Unstaged files are modified files that have not yet been staged for the next commit.  
- These changes have been made in the working directory but have not been added to the staging area.  

<a name="fc"></a>
## Flowchart - File Lifecycle:   

   ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/concepts/images/git_status_flowchart.png)  

   ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/concepts/images/git_status.png)  

<a name="wt"></a>
## Working Tree:  
- The working tree represents the current state of files you are actively modifying within your project directory.  
- It encompasses all files being edited in your project folder, including those tracked by Git and any new files created that Git is not currently monitoring.  
- In brief, the working tree contains the most up-to-date versions of files or their current states.  

   ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/concepts/images/working_tree.png)   
