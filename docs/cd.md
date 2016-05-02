# cd
> change working directory  

`$ cd <path>`  
Change the current working directory of the shell to a relative or absolute path. If you type cd with out any arguments it will take you to your home directory. Use `~` or `$HOME` to references paths from your home directory.

## examples
``` sh
# change current working directory to your home directory

$ cd

# or

$ cd ~

# or

$ cd "$HOME"
```

``` sh
# change current working directory to the relative path client/js/test

$ cd client/js/test
```

``` sh
# change current working directory to the absolute path ~/Downloads

$ cd ~/Downloads

# or

$ cd $HOME/Downloads
```

``` sh
# change current working directory to the absolute path /usr/local/bin

$ cd /usr/local/bin
```
