# Commands:

<a name="top"></a>
- [ git ](#git)  
- [ config ](#config)  
- [ init ](#init)  
- [ clone ](#clone)  
- [ status ](#status)  
- [ add ](#add)
- [ commit ](#commit)  
- [ diff ](#diff)  
- [ log ](#log)  
- [ show ](#show)

<a name="git"></a>
## git:  
- A primary interface for interacting with Git.
- Git is a fast, scalable, distributed revision control system with an unusually rich command set that provides both high-level operations and full access to internals.
- Syntax:
    `git <options>`  
- Few options:
    - **-v**: 
        - This option is used to print the current version.
        - Syntax:
            `git -v`
            `git version`
            `git --version`

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_version.png)  

    - **-h**: 
        - Used to display the synopsis and a list of commonly used commands. It is used along with some command, then it displays the usage of a particular command.
        - Syntax: 
            `git -h`
            `git --help`
            `git <command> -h`
            
            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_help.png)  

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_command_help.png)  

    - **-c <path>**: 
        - This allows us to run Git commands as if we were in a different directory than the current working directory.  
        - Syntax:
            `git -C <repo-path> command`
        - Usage:
            `git -C demo init`
            - Here, demo is the directory which is present inside the current directory and init is the command which is used to initialize the directory into git repo. We can use any other commands as well.  

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_c.png)  

- There are many other options like:  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_options.png)  

<p align="right">
  <a href="#top">▲Home▲</a>
</p>

<a name="config"></a>
## config:  
- Used to set and get the configuration variables.
- Controls various aspects of Git's behaviour like user info, core settings, repo related config etc..
- Syntax:  
    `git config <options>`
- **--list**:
    - Used to get all the config variables along with their variables.
    - Command:
        `git config --list`

        ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_config_list.png)   
    
- **username** and **email**:
    - Before making any commits, make sure to set email and username.
    - Set these using **--global** option as this applies to the current user across all the repos.
    - Syntax:
        - to set globally:
            `git config --global user.email <your-email-address>`
            `git config --global user.name <your-name>` 

        - to get them:
            `git config user.email`
            `git config user.name`

        ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_config_name_mail.png)  

    - We can also set the configuration in a system level **--system** and for a particular repo level **--local**
    - To remove a configuration variable, we can use **--unset**
    - Syntax: 
        `git config --unset <variable>`

        ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_config_unset.png)

- **--edit**:
    - We can edit the config file.  
    - Syntax:  
        `git config --edit`  

<p align="right">
  <a href="#top">▲Home▲</a>
</p>

<a name="init"></a>
## init:
- This turns a local folder that isn't under version control into git repo.  
- Creates an new empty git repo.  
- Also reinitializes an existing repo.  
- Syntax:  
    `git init`   
- During this initialization, a hidden .git folder is created, and this contains all the info that Git uses to manage the project.  

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_init.png)  

- By default, when a local is initialized to git repo, it will be on the **master** branch.  

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_init_master.png)  

- We can also set our own branch name while initializing a repo using:  
    `git init -b <branch-name>`  
    `git init --initial-branch=<branch-name>`  

<a name="clone"></a>
## clone:  
- To create a copy of an existing repo.  
- It also copies all the repo's info like files, commit history, branches, etc..  
- Syntax:  
    `git clone <repo-URL>`  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_clone.png)  

<a name="status"></a>
## status:  
- Used to show the current status of the working directory and staging area of Git repository.  
- It gives info about the files that are untracked, staged and unstaged.  
- Syntax:  
    `git status`  

  ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_status_basic.png)  

<p align="right">
  <a href="#top">▲Home▲</a>
</p>

<a name="add"></a>
## add:  
- Used to track the files.    
- Syntax:  
    `git add filename`  

  ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add.png)  

- All the tracked files will be in the **Staging Area**.    
- Options:   
```
  #path to a specific file or directory  
> git add <path>  

  #all the files in the current directory and its subdirectories  
> git add .  

  #all the files in entire repo/project  
> git add -A  

  #similar to -A option  
> git add --all  

  #all changed files and deleted files except new files  
> git add -u  

  #to track multiple files at once  
> git add <file-name1> <file-name2> <file-name3>  
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_u.png)  

- There's a command that initiates an interactive mode for adding/tracking the files. It opens an interactive staging interface, known as **Interactive Add** or **Patch Mode**. We can choose the changes with a menu-driven interface.  
    Command: `git add -i`  

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_i.png)  

- Options of add interactive mode:  
    1. **status**: shows the status of the files regarding changes made.    

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_i_1.png)  

    2. **update**: adds the specified files to the staged state.  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_i_2.png)  

    3. **revert**: reverts back the staged files to the untracked stage.    

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_i_3.png)  

    4. **add untracked**: adds the untracked files to the staged state.   

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_i_4.png)  

    5. **patch**: picks up the hunks/changes and updates selectively    

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_i_5.png)  

    6. **diff** : view the difference between the HEAD and index  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_i_6.png)  

    7. **quit** : quits from the interactive mode  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_i_7.png)  

    8. **help**: shows the usage of all the options  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_i_8.png)  

- Options for the **--patch or -p** flag:  
    - **y**: confirmation stage this change/hunk    
    - **n**: do not stage this change/hunk  
    - **q**: quit  
    - **a**: stage this change and all the later changes that are made to this file specified  
    - **d**: don't stage this change or any of the later changes that are made to this file specified  
    - **e**: edit the current change manually  
    - **?**: help  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_add_patch.png)  

<p align="right">
  <a href="#top">▲Home▲</a>
</p>

<a name="commit"></a>
## commit:  
- This acts like a **checkpoint** or a **savepoint**  
- This is used to track the changes that are made to a file.  
- Can revert back to the old changes easily using this command.  
- Tracking can be easy using the commit messages.  
- Syntax:  
    `git commit`  
- All the tracked files will be moved from the staged state to the local repo.  
- Using different options:  
    - `git commit` - using this way a commit message terminal will be displayed.  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_commit.png)  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/commit_message_terminal.png)  

    - `git commit -m "Some Commit Message"` - commit using a message flag.  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/commit_m.png)   

    - `git commit -a -m "Some Commit Message"` - can skip the add command as both add and commit can be used in a single command.  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/commit_am.png)  

    - `git commit --amend` - Can replace the most recent commit with a new commit using **--amend** flag. We can give a new commit message in the message terminal.  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/commit_amend.png)  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/commit_amend_message.png)   

<p align="right">
  <a href="#top">▲Home▲</a>
</p>

<a name="diff"></a>
## diff:  
- It is used to view the changes between commits, branches, files, etc..  
- Shows the differences between staging area and the working directory i.e., lists all the changes in the working directory that aren't staged for the next commit.  
- Syntax:
      ```
      git diff
      ```
- `git diff HEAD` - lists all the changes in the working directory since the last commit.  
- `git diff --staged` or `git diff --cached` - lists the changes of the files in the staging area and last commit.  
- `git diff branch1..branch2` or `git diff branch1 branch2` - compares all the files in the mentioned 2 branches.  
- `git diff commit1..commit2` or `git diff commit1 commit2` - compares the files of 2 commits.  
- We can also compare a specific file using: `git diff <file-name>`  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_diff.png)  

- Output:
    - **Compared Files or Diff Header**: 
        - diff --git a/colors.txt b/colors.txt  
        - Shows the names of the files that are being compared  
        - a/colors.txt refers to the original version  
        - b/colors.txt refers to the modified version  
    - **File Metadata or Index Line**:  
        - index a9d1386..fa3e75c 100644  
        - Gives info about the staging area that represents the state of a file in the repo.  
        - a9d1386..fa3e75c refers to the hash values of the 2 versions of file.  
        - 100644 refers to the internal file mode identifier  
    - **Markers or File Change Section**:  
        - --- a/colors.txt and +++ b/colors.txt  
        - represents the original version and modified version of file  
    - **Chunks or Chunk Header**:  
        - @@ -1 +1,2 @@  
        - Info about the lines that are being compared.  
        - -1 indicates the starting line number in the 'a' version  
        - +1,2 indicates the starting line number in the 'b' version (+1) and the number of lines changed (2).  
    - **Changes**:  
        -  red and +yellow  
        - lines that begin with - come from original version.  
        - lines that begin with + come from modified version.  

<p align="right">
  <a href="#top">▲Home▲</a>
</p>

<a name="log"></a>
## log:  
- Displays the commit history and most recent commits are displayed first.  
- Syntax:  
      ```
      git
      ```

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_log.png)  

- `git log --oneline` or `git log --pretty=oneline`: displays the logs in a simplified way.  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_log_oneline.png)  

- `git log -p`: displays the commits along with its particular changes that are made.  

<a name="show"></a>
## show:  
- Displays the detailed info about a specific objects.  
- Objects: commits, tags, branches, tree objects, blob objects, annotated tags...  
- By default, it displays the detailed info about the most recent commit.  
- Syntax:  
      `git show`

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/git/commands/images/git_show.png)  

- Syntax to use a specific object:  
      `git show <object-id>`  

<p align="right">
  <a href="#top">▲Home▲</a>
</p>
