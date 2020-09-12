# Complete Laptop Setup

## Homebrew maintenance

1. `brew update`
2. `brew upgrade`
3. `brew cask upgrade`

## Manual Pre-Setup

1. Install homebrew: https://treehouse.github.io/installation-guides/mac/homebrew # Might need to update Xcode
2. `brew install python3 ansible git`

## Run Ansible Playbook

Git clone this repo, and from the ansible directory:
`ansible-playbook -i inventory.cfg site.yml -c local`

### Breakdown of stages

1. brew install apps
2. pip3 install apps
3. brew cask install apps
4. Shell Scripts:
    * Change default shell to zsh
      * `chsh -s \$(which zsh)`
    * Download and install oh-my-zsh
      * `sh -c "\$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
    * Clone powerlevel10k
      * `https://github.com/romkatv/powerlevel10k.git`
    * Clone nerd-fonts
      * `https://github.com/ryanoasis/nerd-fonts.git`
    * Clone iterm2 design theme
      * `https://github.com/MartinSeeler/iterm2-material-design.git`
    * Copy files over to home and .config
      * `.flake8`
      * `.p10k.zsh`
      * `.zshrc`
      * `nvim directory to ~/.config`
    * Install vim-plug
      * `curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim`
    * Install vim plugins
      * `nvim -c "PlugInstall" or :PlugInstall`
      * `nvim -c "GoInstallBinaries" or :GoInstallBinaries`
      * `nvim -c "CocInstall <args>" or :CocInstall <args>`

### Manual OSX Settings

OSX defaults can change often with upgrades, not worth maintaining this section over the years in ansible

1. Apply source code pro font in iterm -> profile settings
2. iterm2 > preferences > profiles > colors > color presets > import > material-design-colors.itermcolors
3. In Iterm2 preferences -> Keys -> have "cmd/" send "++" to comment out and uncomment using the nerdcommenter extension quickly
4. Other OSX settings:
    * Automatically hide dock
    * General -> Show Scroll Bars -> Always
    * General -> Default Browser -> Brave
    * General -> Uncheck -> Close Windows when quitting an app
    * General -> Uncheck -> Allow Handoff between this mac and other devices
    * Security & Privacy -> Require password immediately after sleep
    * Display -> Uncheck -> Automatically adjust brightness
    * Display -> Uncheck -> True Tone
    * Display -> Nightshift -> Custom
    * Trackpad -> Point & Click -> Secondary Click -> Click in bottom right corner
    * Trackpad -> Scroll & Zoom -> Uncheck -> Scroll Direction Natural
    * Mouse -> Point & Click -> Uncheck -> Scroll Direction Natural
    * Mouse -> Point & Click -> Check -> Secondary click on right side
    * Tracking Speed 5 for both mouse and trackpad
5. Setup SSH keys for work and/or personal repositories
6. Open on login preferences:
    * Google Backup and Sync
    * Alfred
    * Amethyst
    * Coffee Buzz
    * Pock

### Manual App Store Only Installs
1. Todoist
2. Coffee Buzz
3. Be Focused Pro

### Troubleshooting
1. Path in .zshrc, `export ZSH=` might need to be updated if username doesn't match personal
2. ansible_python_interpreter var would need to be updated if python3 isn't in /usr/bin/python3
3. May need to run the command `pip3 install -U neovim` for pynvim interpreter to work
4. Run `:checkhealth` in vim to ensure everything is working smoothly
5. `CocInstall` and `GoInstallBinaries` sometimes seems to not work, re-run those two commands if
that's the case.
