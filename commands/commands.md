### git:  
- A primary interface for interacting with Git.  
- Git is a fast, scalable, distributed revision control system with an unusually rich command set that provides both high-level operations and full access to internals.  
- Syntax:  
    `git <options>`  
- Few options:  
    - **-v**: 
        - This option is used to print the current version.  
        - Syntax:
            ```
            git -v
            ```
            ```
            git version
            ```
            ```
            git --version
            ```

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_version.png)  

    - **-h**: 
        - Used to display the synopsis and a list of commonly used commands. It is used along with some command, then it displays the usage of a particular command.  
        - Syntax: 
            ```
            git -h
            ```
            ```
            git --help
            ```
            ```
            git <command> -h
            ```

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_help.png)  

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_command_help.png)  

    - **-c <path>**: 
        - This allows us to run Git commands as if we were in a different directory than the current working directory.  
        - Syntax:  
            `git -C <repo-path> command`
        - Usage:
            ```
            git -C demo init
            ```
            - Here, demo is the directory which is present inside the current directory and init is the command which is used to initialize the directory into git repo. We can use any other commands as well.  

            ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_c.png)  

- There are many other options like:  

    ![screenshot](https://github.com/saimanasak/git-and-github/blob/main/commands/images/git_options.png)  
