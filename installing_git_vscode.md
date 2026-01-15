## Installing Git on Windows and Mac

Both computere system have different methods to install Git. If you want see the other option for installing Git, go to: https://git-scm.com/install

### Installing Git on a Mac (macOS 10.9 or above) 
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



    






     
    
