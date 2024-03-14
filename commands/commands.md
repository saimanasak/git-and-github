### git:  
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

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_version.png)  

    - **-h**: 
        - Used to display the synopsis and a list of commonly used commands. It is used along with some command, then it displays the usage of a particular command.
        - Syntax: 
            `git -h`
            `git --help`
            `git <command> -h`
            
            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_help.png)  

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_command_help.png)  

    - **-c <path>**: 
        - This allows us to run Git commands as if we were in a different directory than the current working directory.  
        - Syntax:
            `git -C <repo-path> command`
        - Usage:
            `git -C demo init`
            - Here, demo is the directory which is present inside the current directory and init is the command which is used to initialize the directory into git repo. We can use any other commands as well.  

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_c.png)  

- There are many other options like:  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_options.png)  

### config:  
- Used to set and get the configuration variables.
- Controls various aspects of Git's behaviour like user info, core settings, repo related config etc..
- Syntax:  
    `git config <options>`
- **--list**:
    - used to get all the config variables along with their variables.
    - Command:
        ```
        git config --list
        ```

        ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_config_list.png)   
    
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

        ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_config_name_mail.png)  

    - We can also set the configuration in a system level **--system** and for a particular repo level **--local**
    - To remove a configuration variable, we can use **--unset**
    - Syntax: 
        `git config --unset <variable>`

        ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_config_unset.png)

- **--edit**:
    - We can edit the config file.
    - Syntax:
        `git config --edit`

