# Initial Setup
 ### Update and upgrade all packages
 - `sudo apt update`
 - `sudo apt upgrade`

### Install gnome tweak tools
- `sudo apt install gnome-tweak-tool`
- Go to Gnome extensions, install the extension for chrome
  - Install Dash to Dock

### Install restricted formats
- `sudo apt-get install ubuntu-restricted-extras`

### Install Google Chrome
- `wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb`
- `sudo dpkg -i google-chrome-stable_current_amd64.deb`

# Apps from the Pop-Shop
- Telegram Desktop
- Discord
- Visual Studio Code

# Set up terminal
- `sudo apt install zsh`
- `chsh -s $(which zsh)`  // change the shell to zsh
- log out and log back in, no need to restart the pc
- reopen the terminal and select option **2**
- install Oh my zsh via curl or wget
  - sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
  - sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
- open .zshrc file `sudo nano .zshrc`
  - uncomment `export PATH=$HOME/bin:/user/local/bin:$PATH`
  - uncomment `export UPDATE_ZSH_DAYS=3`
  - uncomment `ENABLE_CORRECTION="true"`
- Install zsh autosuggestions `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`
- open .zshrc file `sudo nano .zshrc`
  - add `zsh-autosuggestions`
- type `source ~/.zshrc` to refresh the shell

## Aliases
To set aliases open .zshrc file with nano and go the Aliases section at the bottom
Set these aliases:
- `alias zshconfig="sudo nano ~/.zshrc"`
- `alias srczsh="source ~/.zshrc"`
- 

# Node.js
Version LTS
- `curl -sL https://deb.nodesource.com/setup_lts.x | sudo -E bash -`
- `sudo apt-get install -y nodejs`
Version Current
- `curl -sL https://deb.nodesource.com/setup_current.x | sudo -E bash -`
- `sudo apt-get install -y nodejs`

This commands should install the latest LTS or Current version, if problems occur refer to this link
[https://github.com/nodesource/distributions/blob/master/README.md]

Install also the build tools
- `sudo apt-get install -y build-essential`
Fast clean up
- `sudo apt autoremove`

# Trash Cli
link to the npm package --> [https://www.npmjs.com/package/trash-cli]
- `$ npm install --global trash-cli`
Add an alias to the .zshrc file
- `alias rm=trash`

# Visual Studio Code
## Fonts
- Anonymous Pro [https://fonts.google.com/specimen/Anonymous+Pro]
## Extensions
### Themes/Color
- Just Black
- Material Color Theme
- Bracket Pair Colorizer
### Workflow
- advanced-new-file
- autoclose tag
- autorename tag
- fontsize shortcuts
- toggle quotes
### Intellisense/Autocomplete




