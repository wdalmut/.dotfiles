# Dot Files

The base git alias is in the `.bash_aliases` file

## Do not expose the whole home directory to git

```
config config --local status.showUntrackedFiles no
```

## Use the install

```
curl -Ls https://raw.githubusercontent.com/wdalmut/.dotfiles/master/bin/wdm-install | /bin/bash
```

## Manual restore configurations

```
alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
config checkout
config config --local status.showUntrackedFiles no
```
