# Setup
Helpful files for getting up and running in a new environment

## Install Homebrew
`ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

## Install Sublime
`brew cask install sublime-text`

## Generate a new ssh key
`ssh-keygen -t rsa -b 4096 -C "email@domain.com"`

## Add that new ssh key
```
eval "$(ssh-agent -s)"
ssh-add -K ~/.ssh/id_rsa
```

## (unscripted step) Add your ssh public key to your github account

## Clone this repo
`cd ~ && git clone git@github.com:navenoxin/setup.git`

## Link this repo's ssh config file to the one osx will expect
`ln ~/setup/.ssh/config ~/.ssh/config`

## Link .bash_profile and supporting scripts
```
ln ~/setup/.ssh/config ~/.bash_profile
ln ~/setup/.git-prompt.sh ~/.git-prompt.sh
chmod +x ~/setup/.git-prompt.sh
ln ~/setup/.git-completion.bash ~/.git-completion.bash
chmod +x ~/setup/.git-completion.bash
```

## Update terminal theme
Import `OneDark.terminal` in terminal preferences, set as default

## Link sublime settings
todo
