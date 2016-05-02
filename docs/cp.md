# cp
> copy files and directories  

`$ cp <flags> <source file path> <target file path>`  

`cp` is used to copy a file or a directory. When you copy a directory it will copy all of the contents of the directory as well.

## warning
* `cp` wil overwrite an existing target file, and you can not get it back.
* when copying a directory make sure the source path does not end with a `/`, this will copy only the contents of that directory
 * **good** `~/Desktop`
 * **bad** `~/Desktop/`


## important flags
* `-n` do not overwrite an existing file.
* `-R` recursively copy (used to copy directories)
* `-v` cause cp to be verbose, logging files as they are copied

## examples
``` sh
# make a backup copy of ~/.bashrc called .bashrc.backup

cp ~/.bashrc ~/.bashrc.backup
```
``` sh
# copy ~/.eslintrc into the current directory

$ cp ~/.eslintrc ./
```

``` sh
# make a copy of the directory ~/Desktop/image_icons
# into ~/code/portfolio/

$ cp -R ~/Desktop/image_icons ~/code/portfolio/image_icons
```
