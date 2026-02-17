## Creating a Repository in VS Code

### Step 1: Open a New Window
1. Click on **File** > select **New Window**

### Step 2: Select Your Project Folder

1. Under **Explorer** or **Version Control**, click on **Open Folder**
2. An Explorer (Windows) or Finder (Mac) window will open

![Screenshot of VS Code interface](screenshots/vs_code_explore_closeup.png) 

3. Navigate to your **Documents** folder
4. Either:
   - Create a new folder for your project, OR
   - Select an existing project folder

![Screenshot of VS Code interface](screenshots/vs_code_finder.png) 

5. Click to open the folder
6. A new VS Code window will open (don't be alarmed - this is normal!)

### Step 3: Initialize Version Control
Click on the **Source Control** icon in the sidebar. You'll see two options:

![Screenshot of VS Code interface](screenshots/vs_code_sourcecontrol_options.png) 

#### Option A: Local Git Only (No GitHub Account Needed)
- Click **Initialize Repository**
- Your repository is now tracking changes locally on your computer
- Use this for: personal projects, learning Git, working offline

#### Option B: Publish to GitHub (Requires GitHub Account)
- Click **Publish to GitHub**
- Use this for: collaborating with others, cloud backup, public projects, contributing to open source, code review via pull requests

### Step 4: Create Your First File
1. Create a new file in your project (e.g., `README.md` or `index.html`)
2. Add some content to the file

### Step 5: Make Your First Commit

![Screenshot of VS Code interface](screenshots/vs_code_source_control_testfile.png) 

#### If you chose Option A (Local Git):
1. Go to the **Source Control** panel
2. You'll see your new file listed under "Changes"
3. Click the **+** icon to stage the file
4. Type a commit message in the text box (e.g., "Initial commit")
5. Click the **✓ Commit** button

**Optional:** To publish to GitHub later:
- Click **Publish Branch** in the Source Control panel
- You'll be prompted to sign in to GitHub
- Choose whether to make your repository **Private** or **Public**

#### If you chose Option B (Publish to GitHub):
1. Add a commit message when prompted (e.g., "Initial commit")
2. Choose whether to make your repository **Private** or **Public**
3. VS Code will automatically:
   - Create the repository on GitHub
   - Commit your files
   - Push them to GitHub

---

### 📌 Key Difference:
- **Local Git** = Version control on your computer only
- **GitHub** = Your code is also stored online and can be shared