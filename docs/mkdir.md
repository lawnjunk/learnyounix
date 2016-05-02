# mkdir
> make directories

`$ mkdir <flags> <dirpath>`  

The mkdir utility is used to create empty directories.

## important flags
* `-p` create intermediate directories as required

## examples
``` sh
# create a directory named 'css' in the current working directory

$ mkdir css
```
``` sh
# create the directory client/js/test and any of its parent directories
# if they are needed.

$ mkdir -p client/js/test
```
