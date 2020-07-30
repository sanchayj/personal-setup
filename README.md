# Install Basic Software

install homebrew: https://treehouse.github.io/installation-guides/mac/homebrew # Might need to update Xcode
install iterm2: https://www.iterm2.com/

brew install go  
brew install python3  
pip3 install flake8-black  
pip3 install pytest  
pip3 install isort  
brew install ruby  
brew install pylint  
brew install watchman  
brew install fzf  
brew install tmux  
brew install neovim  
brew install yarn  
brew install zsh zsh-completions  
brew install yamllint # for ze yaml linting needs  
brew install exercism  

chsh -s \$(which zsh) # Will change default shell to zsh, requires password

sh -c "\$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" # Install oh-my-zsh

# Install Themes

git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
ZSH_THEME="powerlevel9k/powerlevel9k" in .zshrc

Install Source Code Pro for Powerline font (semibold)
  You'll need to get the nerd font version from vim-devicons for compatibility with nerdtree
Apply font in iterm -> profile settings

In Iterm2 preferences -> Keys -> have "cmd/" send "++" to comment out and uncomment using the nerdcommenter extension quickly

Download iterm2 Material Design theme: https://github.com/MartinSeeler/iterm2-material-design

Run command in iterm for downloading plug.vim (vim-plug): curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

Create a directory: ./config/nvim/ and add your init.vim file to it
Run :PlugInstall inside init.vim to install plugins

From inside Vim, run :CocInstall coc-python coc-json coc-snippets coc-yaml coc-vimlsp coc-tsserver coc-go coc-solargraph coc-rust-analyzer coc-sh coc-markdownlint coc-sql coc-html

Put .flake8 file in the home directory

for COC guide use: https://www.chrisatmachine.com/Neovim/04-vim-coc/ 

Manage packages for:
brew  
pip3  
plug (vim)  
coc (vim)  
app store  
system software updates  

Backup files:  
~/.config/nvim/  

Useful applications:  
Coffee Buzz  
Amethyst  
Backup and Sync (Google Drive)  
Raindrop.io  
Notion  
Todoist  
Alfred 4  
Brave (browser)  
iterm2  
Office Suite  
Pock  
