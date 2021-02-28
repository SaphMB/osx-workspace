# osx-workspace

Scripting the setup of a macOSX computer.

## Initial set-up

```
git clone https://github.com/SaphMB/osx-workspace
cd osx-workspace
./shell_setup | bash
```
This will install Homebrew, all Homebrew packages and oh-my-zsh.

```
./go_packages
./ruby_packages
```

Together, these will install install rvm and the latest stable version of Ruby, as well as all regularly-used Ruby and Go packages.

### Configs

#### zsh
Create a symlink from the ./zshrc in this repo to ~./zshrc.

#### Git config
Create a symlink from the ./gitconfig in this repo to ~./gitconfig.

#### VSCode
* Install the code-settings-sync VSCode plugin
* Download files uploaded to Gist with `Shift + Option + U`, providing a github api token when prompted

#### Vim config

Create a directory for packages and update ~/.vimrc with the .vimrc in this repo.
```
mkdir ~/.vim/plugged
```

Install packages
```
vim ~/.vimrc
:PlugInstall
```
