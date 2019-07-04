# My vim Files

This is my repository to store vim configuration files

## Inspirations

- http://vimcasts.org/episodes/synchronizing-plugins-with-git-submodules-and-pathogen/

## Usage

1. Clone: `git clone https://github.com/ausuwardi/vim-files.git vim-files`
2. Link `.vimrc`: `ln -s $PWD/vim-files/vimrc $HOME/.vimrc`
3. Link `.vim`: `ln -s $PWD/vim-files $HOME/.vimrc`
4. Install vim plugins submodule: `cd vim-files && git submodule update --init`

## Installing New Plugins

To install new plugins, add as submodule inside bundle subdirectory:

```
cd vim-files
git submodule add https://github.com/vim-syntastic/syntastic.git bundle/syntastic
```

## Updating A Plugins

To update one plugin:

```
cd vim-files/bundle/nerdtree
git pull origin master
```

## Update All Plugins

To update all installed plugins in one run:

```
cd vim-files
git submodule foreach git pull origin master
```

