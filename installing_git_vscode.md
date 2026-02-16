## Installing Git on Windows and Mac

Both computer systems have different methods to install Git. If you want to see other installation options, go to: https://git-scm.com/downloads

---

## Installing Git on Mac (macOS 10.9 or above)

### Option 1: Quick Install (Easiest)

1. Open **Terminal** (find it in Applications → Utilities)
2. Type: `git --version` and press Enter
3. If Git isn't installed, macOS will prompt you to install it
4. Click **Install** and follow the prompts

**That's it!** Verify it worked by typing `git --version` again.

---

### Option 2: Install with Homebrew (Recommended for developers)

**What is Homebrew?** It's a package manager that makes installing and updating software easier on Mac.

#### Step 1: Check Where You Are

Open Terminal and type:

```bash
pwd
```

This shows your current location (usually `/Users/your-username`)

#### Step 2: Install Homebrew

Copy and paste this entire command into Terminal:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Press Enter and follow any prompts (you may need to enter your password)

#### Step 3: Verify Homebrew Installed

Type:

```bash
which brew
```

You should see: `/opt/homebrew/bin/brew` (or `/usr/local/bin/brew` on older Macs)

#### Step 4: Install Git

Type:

```bash
brew install git
```

#### Step 5: Verify Git Installed

Type:

```bash
which git
```

You should see: `/opt/homebrew/bin/git`

Then check the version:

```bash
git --version
```

You should see something like: `git version 2.52.0`

---

### Keeping Git Updated (Homebrew users)

**Update only Git:**

```bash
brew upgrade git
```

**Update everything installed with Homebrew:**

```bash
brew upgrade
```

**Update a specific package:**

```bash
brew upgrade <package_name>
```

(In Homebrew terminology, packages are called "formulas")

---

## Installing Git on Windows

[Your Windows instructions would go here]

---

### Quick Troubleshooting

**Mac: Command not found?**

- Close and reopen Terminal
- Try the command again

**Mac: Which option should I choose?**

- **Option 1** is faster and simpler
- **Option 2** is better if you plan to install other development tools

**Homebrew installation takes a long time?**

- This is normal! It can take 5-10 minutes
- Don't close the Terminal window

### Quick Troubleshooting

**Mac: Command not found?**

- Close and reopen Terminal
- Try the command again

**Mac: Which option should I choose?**

- **Option 1** is faster and simpler
- **Option 2** is better if you plan to install other development tools

**Homebrew installation takes a long time?**

- This is normal! It can take 5-10 minutes
- Don't close the Terminal window

## Installing Git on Windows

### Step 1: Download Git

Go to https://git-scm.com/download/windows and download the installer.

### Step 2: Run the Installer

1. Double-click the downloaded file
2. Click **Yes** when Windows asks if you want to allow the app to make changes

### Step 3: Installation Options

You'll see many setup screens. Here's what to do:

**Most screens: Just click "Next"** - the default options work great!

**Pay attention to these 3 screens:**

1. **Choose your editor**
   - If you use Visual Studio Code, select "Use Visual Studio Code as Git's default editor"
   - Otherwise, keep the default and click "Next"

2. **Adjusting your PATH environment**
   - Select **"Git from the command line and also from 3rd-party software"**
   - This lets you use Git everywhere (Command Prompt, PowerShell, VS Code, etc.)

3. **Choosing the default branch name**
   - Select "Override the default branch name for new repositories"
   - Type **main** in the box
   - (This matches what GitHub uses)

**For all other screens:** The defaults are fine - just click "Next"

### Step 4: Finish Installation

Click **Install**, wait for it to complete, then click **Finish**.

### Step 5: Verify It Worked

1. Open Command Prompt or PowerShell
2. Type: `git --version`
3. You should see something like: `git version 2.43.0`

**You're done!** Git is now installed and ready to use.

---

### Quick Troubleshooting

**Don't see a version number?**

- Close and reopen your terminal/command prompt
- Try again with `git --version`
