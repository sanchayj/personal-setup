# Install Basic Software

## Homebrew maintenance

1. `brew update`
2. `brew upgrade`
3. `brew cask upgrade`

## Manual

1. Install homebrew: https://treehouse.github.io/installation-guides/mac/homebrew # Might need to update Xcode
2. `brew install python3 ansible git`

## Ansible

1. `brew install <apps>`
    * go
    * ruby
    * pylint
    * watchman
    * fzf
    * tmux
    * neovim
    * yarn
    * zsh
    * zsh-completions
    * yamllint
    * ripgrep
    * minikube
2. `pip3 install <apps>`
    * flake8-black
    * pytest
    * isort
3. `brew cask install <apps>`
    * alfred
    * amethyst
    * brave-browser
    * google-backup-and-sync
    * microsoft-office
    * pock
    * notion
    * iterm2
    * raindropio
    * docker
    * spotify
4. Shell Scripts:
    * chsh -s \$(which zsh) # Will change default shell to zsh, requires password
    * sh -c "\$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" # Install oh-my-zsh
    * git clone your personal-setup repo, place all files in proper directories, nvim in .config
    * git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
    * git clone source code pro for powerline and install it on mac?
    * Download iterm2 Material Design theme: https://github.com/MartinSeeler/iterm2-material-design
    * Run command in iterm for downloading plug.vim (vim-plug): curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
    * :PlugInstall and :GoInstallBinaries inside a vim file
    * From inside Vim, run :CocInstall coc-python coc-json coc-snippets coc-yaml coc-vimlsp coc-tsserver coc-go coc-solargraph coc-rust-analyzer coc-sh coc-markdownlint coc-sql coc-html

### Manual OSX Settings
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

### Manual App Installs
1. Todoist
2. Coffee Buzz
3. Be Focused
