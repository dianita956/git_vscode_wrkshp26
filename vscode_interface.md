## Walk through of VS Code Interface 

![Screenshot of VS Code interface](screenshots/vs_code_gui.png) 

1. **Editor** - The main area where you write and edit your code/text files
2. **Terminal** - Built-in command line (same as your computer's terminal!)
3. **Explorer** - Your project files and folders
4. **Activity Bar** - Icon strip on the far left - click to change views
5. **Accounts** - Sign in to GitHub (we'll use this later!)
6. **Status Bar** - Bottom bar showing: branch name (left), file info (right)

---
## The Main Component, let's break it down

### 1. **Activity Bar** (left side bar)

This is your navigation hub. Click these icons to change what appears in the side bar:

- **Explorer**
- **Search**
- **Source Control**
- **Extensions** 


### 2. **Editor Area** the big space in the middle

This is where you write and edit your files. 

**things to know:**
- each file opesn in a **tab** at the top
- you can have multiple files open at once
- you can split the editor to see two files side-by-side. (view » editor layout or top right corner icons)

### 3. **Terminal Panel**, the bottom section

Remember those terminal commands from the creating a repository via terminal activity? You can run them right here too! 

**how to open it:** 
- menu: **Terminal » New Terminal**

**Why use the integrated terminal?**
- you don't have to switch between windows
- it automatically opens in your project folder
- you can see your code and terminal at the same time

### 4. **Status Bar**

This bar shows important information about your current file and project.

#### **Left side of Status Bar:**
- **Branch name** (example: `main` or `master`)
    - this tells you which Git branch you are on
    - click it to switch branches

#### **Right Side of Status Bar:** 
- Line and column number (where your cursor is)
- Spaces or Tab settings
- File encoding (usually UTF-8)
- Language mode (Markdown, Javascript, Python, etc.)

---

## Source Control

### **How to Open it:**
1. Click the **Source Control icon** in the Activity Bar (left side bar)

### **What you will see in Source Control view:**

```
Source Control
├── Message box (at the top)
├── ✓ Commit button (checkmark)
├── ...More options (three dots menu above the message box)
├── 📁 Changes (files you have modified)
│   ├── 'M' modified file [+ icon to stage]
│   ├── 📁 Staged Changes (ready to commit)
│   └── M staged file [- icon to unstage]
└── No changes = "no changes" message
```
#### **Message Box**
- Type your commit message here
- same as: `git commit -m "your message"

#### *Changes Section**
- Shows files you've **modified** but not staged yet
- Each file has a **+ icon** next to it
- Clicking + = stages the file (same as `git add filename`)

#### **Staged Changes Section**
- Shows files ready to commit
- Each file has a **- icon** next to it
- Clicking - = unstages the file

#### **Commit Button (✓ Checkmark)**
- Click this to commit your staged changes
- Only works if you've typed a commit message!
---

## Understanding file status indicators

When you look at files in the Source Control view, you will see letters next to them:

| Letter | Meaning | What Happened |
|--------|---------|---------------|
| **U** | Untracked | New file Git doesn't know about yet |
| **M** | Modified | You changed an existing file |
| **A** | Added | File is staged (ready to commit) |
| **D** | Deleted | You deleted a file |
| **R** | Renamed | You renamed a file |

You'll also see **colors**:
- 🟢 **Green** = New or added
- 🟠 **Yellow/Orange** = Modified
- 🔴 **Red** = Deleted
---

## The Asterisk (*) - Your Uncommitted Changes Alert

### **Look at the Bottom-Left Status Bar**

You'll see your branch name (like `main`). Sometimes you'll see an **asterisk (*)** next to it:

**Example:** `main *`

### **What Does the * Mean?**
- You have **uncommitted changes** in your working directory
- Your files are different from your last commit
- Git is saying: "Hey! You have unsaved work!"

### **When Does It Appear?**
- ✓ You modified a file (even if not staged)
- ✓ You staged changes but haven't committed
- ✓ You deleted files

### **When Does It Disappear?**
- ✓ You commit your changes
- ✓ You discard/undo your changes
- ✓ Your working directory matches your last commit

### **Try It Yourself!**
1. Open any file and make a change
2. Look at the Status Bar → See the `*` appear next to your branch
3. Save the file (`Cmd+S` or `Ctrl+S`)
4. The `*` stays! (because you haven't committed)
5. Stage and commit the change
6. Watch the `*` disappear! ✨

**Think of it as:** The asterisk is like the "unsaved changes" indicator in a document, but for your entire Git repository!
---

## Terminal vs VS Code Visual Interface

Remember the terminal commands from `activity_instructions.md`? Here's how they translate to VS Code:

| What You Want | Terminal Command | VS Code Action |
|---------------|------------------|----------------|
| Check status | `git status` | Open Source Control view |
| Stage a file | `git add filename` | Click **+** icon next to file |
| Stage all files | `git add .` | Click **+** icon in "Changes" header |
| Unstage a file | `git restore --staged filename` | Click **-** icon next to file |
| Commit | `git commit -m "message"` | Type message + click **✓** |
| See what changed | `git diff` | Click on the file in Changes |
| View log | `git log` | Use Timeline view or GitLens extension |

**Both ways work!** Use whichever you prefer. Many developers use both:
- Terminal for quick commands
- VS Code interface for visual feedback and staging specific changes
---

## Viewing Changes (Diff View)

Want to see exactly what you changed in a file?

### **How to View Changes:**
1. Go to Source Control view
2. Click on any file in the "Changes" section
3. Split view opens:
   - **Left side** = Old version (before your changes)
   - **Right side** = New version (with your changes)

### **What You'll See:**
- 🔴 **Red background** = Lines you deleted
- 🟢 **Green background** = Lines you added
- No highlight = Lines that didn't change

This is the visual version of `git diff`!
---

## Quick Practice Checklist

Before moving on, make sure you can:

- [ ] Identify the Activity Bar, Editor, Terminal, and Status Bar
- [ ] Open the Source Control view
- [ ] See your current branch name in the Status Bar
- [ ] Understand what the asterisk (*) means
- [ ] Stage a file using the + icon
- [ ] Unstage a file using the - icon
- [ ] View the diff of a changed file
- [ ] Type a commit message and commit
---


