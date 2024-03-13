## Version Control System:  
- It is also known as Versioning or Source Control or Source Code Management.  
- It is a software that helps to manage and track changes to the files over time.  
- It allows users to revisit the earlier versions of the files, compares the changes between the versions, undo the changes and so on...  
- Generally, the main purpose is to facilitate the collaboration among the multiple developers working on a shared project and to keep the history of the changes that are made in the project.  

### Features of VCS:  
- Can tracks changes made to a file i.e., Versioning.  
- Creates a checkpoint for a file at particluar state.  
- Can ignore the files that we don't want to track.  
- Can go back to the previous states of a file.  
- Commits, Branching, Collaboration...  

### Why?  
- Easy to use  
- Collaboration  
- Revert back changes / Rollback  
- Versioning  
- Recovery and Backup  
- Traceability / Compare changes  
- Quality of Code  
- Low Overhead  

### Different types:    
1. **LCVS**  
    - Local Version Control System  
    - It is very simple compared to other VCS.  
    - It involves a simple database or a repository which is located locally, this repo stores all the versions of a file and additional info like commit messages and its timestamps etc..  
    - And that is how all the changes made to files are tracked within this local database.  
    - There's no remote server in this case i.e., no sharing of the files happen here.  
    - Examples:  
        - Revision Control System (RCS)  
        - Source Code Control System (SCCS)  
        - Version SourceSafe (VSS)  
    - Limitations:  
        - No collaboration  
        - Risk of data loss  
        - No remote access  
        
    ![LCVS](https://github.com/saimanasak/git-and-github/blob/main/vcs/images/LVCS.drawio.png)  
