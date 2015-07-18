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

## Clone my dotfiles

```
cd $HOME
git clone git@github.com:dafang/dotfiles.git .dotfiles
```

Then run `fresh install` to configure local shell environment.

## Useful tools

- [zgen](https://github.com/tarjoilija/zgen)
- [antigen](https://github.com/zsh-users/antigen)
- [awesome-zsh-plugins](https://github.com/unixorn/awesome-zsh-plugins#oh-my-zsh)

Thanks to:

- [jasoncodes](https://github.com/jasoncodes/dotfiles)
- [cowboy dotfiles](https://github.com/cowboy/dotfiles)
- [mathiasbynens dotfiles](https://github.com/mathiasbynens/dotfiles)
- [twe4ked dotfiles](https://github.com/twe4ked/dotfiles)
