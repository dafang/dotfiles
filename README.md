# My dotfiles with [fresh](https://github.com/freshshell/fresh)

## Install and configure `fresh`

```
bash -c "`curl -sL get.freshshell.com`"
```

This will:

- Create a ~/.fresh directory.
- Clone the latest version of fresh into ~/.fresh/source/freshshell/fresh.
- Create a ~/.freshrc file.

You will need to manually add `source ~/.fresh/build/shell.sh` to your shell config.

## Install [vim-plug](https://github.com/junegunn/vim-plug)

`curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim`
    
## Install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) and [zgen](https://github.com/tarjoilija/zgen)

Install oh-my-zsh:

`sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

The [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) is leverage the [zgen](https://github.com/tarjoilija/zgen) to manage the zsh plugins. No need to install `zgen` as our dotfiles contains the zgen executor bin file.

Each time if you updated the `.dotfiles/shell/oh-my-zsh/zshrc` file, you need to run `zgen reset` then `zgen save`.

## Clone my dotfiles

```
cd $HOME
git clone git@github.com:dafang/dotfiles.git .dotfiles
```

Then 

```
rm -rf ~/.freshrc
ln -s ~/.dotfiles/freshrc ~/.freshrc
rm -rf ~/.zshrc
```

Then run `fresh install` to configure local shell environment.

Each time if you have modified the dotfiles, you can run `fresh update` to update them.

## Install vim plugins

Run following commands:

```
vim
```

Then, `:PlugInstall`

## Install powerline

See [powerline](https://powerline.readthedocs.io/en/latest/)

Then setup your iTerm fonts to one of the powwerline fonts:

![powerline fonts](https://user-images.githubusercontent.com/207689/34072433-6a95aee0-e2c2-11e7-9693-a88729dbd29d.png)

## Install [HomeBrew](http://brew.sh/) on Mac OS [Only required on Mac]

`ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

Then run `./brew.sh` to install brew packages.

## Useful tools

- [zgen](https://github.com/tarjoilija/zgen)
- [antigen](https://github.com/zsh-users/antigen)
- [awesome-zsh-plugins](https://github.com/unixorn/awesome-zsh-plugins#oh-my-zsh)

Thanks to:

- [jasoncodes](https://github.com/jasoncodes/dotfiles)
- [cowboy dotfiles](https://github.com/cowboy/dotfiles)
- [mathiasbynens dotfiles](https://github.com/mathiasbynens/dotfiles)
- [twe4ked dotfiles](https://github.com/twe4ked/dotfiles)
