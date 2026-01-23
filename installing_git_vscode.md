## Installing Git on Windows and Mac

Both computere system have different methods to install Git. If you want see the other option for installing Git, go to: https://git-scm.com/install

### Installing Git on Mac (macOS 10.9 or above) 
For Mac I will demo two installation ways:

1. Simply run `git --version` from the terminal, and it will prompt you to install it. Follow the instruction since I am not familiar with install Git this way. 

### How i installed Git on Mac

1. open a terminal window, run:

`pwd` let make sure that we know our PATH and its the right path we want to be on

Install **homebrew** and homebrew is a package manager designed for macOS and Linux systems to help simplify installing, updating, and managing software. Install homebrew by run this command: 

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Let's check the brew install type `which brew` and returns `/opt/homebrew/bin/brew`

Once homebrew is installed, we can install git. 

2. To install Git run:

`brew install git`

3. Let's verify the Git install 

    run: `which git` 
    return: `/opt/homebrew/bin/git`

4. Let's check Git version

    run: `git --version`
    returns your version of Git. Latest version is 2.52.0

5. How to install the latest Git version with homebrew

    `brew upgrade git`

   and to ensure homebrew, Git, and any future packages install need to upgrade, run:

   `brew upgrade` 

   for specific package:

   `brew upgrade <package_name>` 

   tho using homebrew terminology, it is `brew upgrade <formula>`  

## Installing Git on Windows

1. download the excutable file from https://git-scm.com/install/windows

2. follow installation prompts but still pay attention the install path. 

3. You will be asked: "Do you want to allow this app to make changes to your device?" click yes to allow git to be installed. 
    - Setup steps:
        - install Git into the following folder. 
        - which components should be installed? I click next... :) 
        - create the program's shortcut in the followinf Start Menu folder. there is check box, bottom left of the wundow, in case you don't want to create short cut path to start menu folder. Shortcut make it easy to find. 
        - which editor would you like Git to use > select > Use Visual Studio Code as Git's editor
        - What would you like Git to name the initial branch after "git init"? it personal choice between 'let Git decide' or 'Override the deflaut branch name for new repositories." I prefer 'main' branch for a new repository. 
        - how would you like to use Git from the command line? i recommend the option "Git from the command line and also from 3rd party software." Editors like VS Code are 3rd party software. 
        - which secure shell client program would you like Git to use? select 'use bundled OpenSSH' since it comes with Git and there additional setup needed. 
        - Which SSL/TLS library would you like Git to use for HTTPS connections? 
        - How should Git treat line endings in text files? 
        - which terminal emulator do you want to use with your Git Bash?
        - what should 'git pull' do by default?
        - which credential helper should be configured?
        - which features would you like to enable? 

### Verify install

1. 
    
