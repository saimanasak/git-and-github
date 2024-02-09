- Git was designed to run on a Unix-based interface (Ex: Bash)  
- Git Bash is a tool that gives a Bash experience on a Windows machine.   

#### Steps to install Git Bash on Windows:  
1. Download the executable (.exe) file from the Git official site - [Git Link](https://git-scm.com/downloads)  
2. Once downloaded, run the executable file.  
3. Can install with the default values or can be changed.  
4. Once installation is done, check the version of the git using:  
    `git --version` or `git version`  

#### Installing on Servers:  
- Git can be installed on different platforms like Ubuntu, CentOS, etc...  
- [Server Link](https://github.com/git-guides/install-git)  
- Commands to download on Ubuntu server:  
```
#command to download/refresh the local package index  
> sudo apt-get update  

#command to install git  
> sudo apt-get install git-all  

#command to check git version  
> git version
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/screenshots/git_version.png)  

#### Configuring Git:  
- Git can be configured using the name and an email.  
- Commands to configure:  
```
#command to configure name globally  
> git config --global user.name <user-name>  

#command to get the user name that is set  
> git config user.name  

#command to configure email globally  
> git config --global user.email <email-address>    

#command to get an email address that is set  
> git config user.email  
```