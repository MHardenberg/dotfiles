# dotfiles

## Install:
echo ".dotfiles" >> .gitignore

git clone --bare <remote-git-repo-url> $HOME/.dotfiles

alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'

config config --local status.showUntrackedFiles no

config checkout


See https://www.ackama.com/what-we-think/the-best-way-to-store-your-dotfiles-a-bare-git-repository-explained/
