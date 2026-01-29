## Activity Instructions

### Let's create a repository via terminal

#### ***Can't see the terminal?*** Go to the menu and click on Terminal > New Terminal
---

Steps:

### 1. check your current working directory/folder by typing:
    - Mac/Linux: `pwd`
    - Windows: `cd`

### 2. creating a new directory/folder (_same commands for Mac and Windows_)

   ```bash
   mkdir git-workshop  # creates a new folder
   cd git-workshop     # changes into that folder
   git init            # initalizes Git repository
   ```

   ### Template 
        mkdir <**foldername**> _creates a new folder/directory_
        cd <**foldername**> _changes the current working directory to the specificed folder._
        git init - _initates a new Git repository_

### 3. check the status of your Git repository:
    ```bash
    git status 
    ```
    
    **_The double-checker, see what you added and what's changed_**

### 4. a typical Git workflow: add, stage, and commit plus the commit message
```bash
   git add activity_instructions.md 
   git commit -m "init repo first commit"
```
### Template 
```
        git add <filename>
```
**_psst-note_** about commit message: Keep message **detailed** and short. It's about documenting changes made, status updates, issues fixed, a mental note to remind yourself and others **what** you changed **and why**.

- **examples of commit messages:**
    - "fix login button not responding on mobile"
    - "add user profile image upload feature"
    - "update README with installation steps"

**don't be me(guilty):** "wishing for the best" :D 

### 5. Review Git changes (like checking your work in Math)
Three ways on to view the log: 

    git log
    
 Very detail log, provides: commit id, author, date, message
   
    git log --oneline 

Short and sweet: first 7 characters of commit id and message
 