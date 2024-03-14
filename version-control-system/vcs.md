# Version Control System:  

<a name="top"></a>
- [ Intro ](#intro)
- [ Features of VCS ](#features-of-vcs)
- [ Why VCS? ](#why)
- [ Different Types ](#different-types)
    - [ Local Version Control System ](#1-lvcs)
    - [ Centralized Version Control System ](#2-cvcs)
    - [ Distributed Version Control System ](#3-dvcs)
- [ Why DVCS? ](#why-dvcs)

<a name="intro"></a>
### Intro:  
- It is also known as Versioning or Source Control or Source Code Management.  
- It is a software that helps to manage and track changes to the files over time.  
- It allows users to revisit the earlier versions of the files, compares the changes between the versions, undo the changes and so on...  
- Generally, the main purpose is to facilitate the collaboration among the multiple developers working on a shared project and to keep the history of the changes that are made in the project.  

<a name="features"></a>
### Features of VCS:  
- Can track changes made to a file i.e., Versioning.  
- Creates a checkpoint for a file at particluar state.  
- Can ignore the files that we don't want to track.  
- Can go back to the previous states of a file.  
- Commits, Branching, Collaboration...  

<a name="why"></a>
### Why?  
- Easy to use  
- Collaboration  
- Revert back changes / Rollback  
- Versioning  
- Recovery and Backup  
- Traceability / Compare changes  
- Quality of Code  
- Low Overhead  

<p align="right">
  <a href="#top">▲Home▲</a>
</p>

<a name="types"></a>
### Different types:    
- There are three types of Version Control Systems, each offering unique features and workflows:  
    1. Local Version Control System  
    2. Centralized Version Control System  
    3. Distributed Version Control System

<a name="lvcs"></a>
### 1. **LVCS**  
- Local Version Control System  
- It is very simple compared to other VCS.  
- It involves a simple database or a repository which is located locally, this repo stores all the versions of a file and additional info like commit messages and its timestamps etc..  
- And that is how all the changes made to files are tracked within this local database.  
- There's no remote server in this case i.e., no sharing of the files happen here.  
- Examples:  
    - Revision Control System (RCS)  
    - Source Code Control System (SCCS)  
    - Version SourceSafe (VSS)  
- Advantages:  
    - Simple  
    - Speed  
    - Offline access  
    - No dependencies  
    - Low overhead  
- Limitations:  
    - No collaboration  
    - Risk of data loss  
    - No remote access  

    ![LVCS](https://github.com/saimanasak/git-and-github/blob/main/vcs/images/LVCS.png)  

<p align="right">
  <a href="#top">▲Home▲</a>
</p>

<a name="cvcs"></a>
### 2. **CVCS**  
- Centralized Version Control System  
- There's a single, central repo which stores all the versions of files and thier history as well.  
- Developers can checkout the files from this central repo to work on them, and then changes are committed back to the central server.  
- i.e., all the users will have their own working copy, whenever the changes are made they get reflected directly in the central repo that means files are affected knowingly or unknowingly.  
- Examples:  
    - Subversion (SVN)  
    - Perforce (Helix Core)  
    - Microsoft Team Foundation Version Control System (TFVC)  
    - Apache Concurrent Version System (CVS)  
- Advantages:  
    - Centralized management  
    - Versioning and history  
    - Access control  
    - Collaboration  
- Limitations:  
    - Single point of failure  
    - Network dependency  
    - Limited offline access  
    - Potential data loss  
     
    ![CVCS](https://github.com/saimanasak/git-and-github/blob/main/vcs/images/CVCS.png)    

<p align="right">
  <a href="#top">▲Home▲</a>
</p>

<a name="dvcs"></a>
### 3. **DVCS**  
- Distributed Version Control System  
- It allows multiple users to collaborate on a project by maintaining a distributed copy of the whole repo on each user's local.  
- Here, all users will have complete history of project that includes branches, commits, and are stored locally.  
- Can make changes without affecting the remote repo.  
- Work flow:  
    `User ----> Commit changes to local repo ----> Push the changes to remote repo`  
- Examples:  
    - Git  
    - Mercurial  
    - Bazaar  
    - Darcas  
- Advantages:  
    - Decentralization  
    - Offline work  
    - Redundancy  
    - Effective collaboration  
    - Security  
    - Flexibility  
- Limitations:  
    - Risk of conflicts  
    - Potential for fragmentation (if not managed carefully)
    
    ![DVCS](https://github.com/saimanasak/git-and-github/blob/main/vcs/images/DVCS.png)    

<a name="why dvcs"></a>
### Why DVCS?  
- High Felixibility
- Faster Performance
- Enhanced Collaboration
- Decentralized
- Offline Work  

<p align="right">
  <a href="#top">▲Home▲</a>
</p>
