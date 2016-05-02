# ~/.bashrc and ~/.bash\_profile
> configuration files for bash

The **~/.bashrc** and the **~/.bash\_profile** are bash scripts that are sourced by bash to help configure the bash environment.

## ~/.bash\_profile
The **~/bash\_profile** is used to configure your shell at login. Which means when you login to a computer via the shell, after you type your username and password in the **~/.bash\_profile** is sourced to configure bash.  

Unfortunately OS X is an exception to this rule. The Terminal on osx will run the **~/.bash\_proflie** every time you create a new window.

## ~/.bashrc
The **~./bashrc** is use to configure your bash every time you open a new terminal, or type the word bash.

## maintain a single configuration file
In order to maintain a single configuration file I create a **~/.bashrc** file will all my configuration in it. Then I create a [symbolic link](https://en.wikipedia.org/wiki/Symbolic_link) from **~/.bash\_profile** to **~/.bashrc**.  

To create [symbolic link](https://en.wikipedia.org/wiki/Symbolic_link) to have **~/.bash\_profile** point to **~/.bashrc** run the following commands

``` sh
# backup your ~/bash_profile

$ mv ~/.bash_profile ~/.bash_profile.backup

# make a symbolic link from ~/.bash_profile to ~/.bashrc

$ ln -s ~/.bashrc ~/.bash_profile
```
