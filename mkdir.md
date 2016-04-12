# mkdir
> make directories

`$ mkdir <flags> <dirpath>`  

The mkdir utilit is used to create empty directories.

## important flags
* `-p` create intermediate directories as required

## exampes
``` sh
# create a directory named 'css' in the current working directory

$ mkdir css
```
``` sh
# create the directory client/js/test and any of its parrent directorys 
# if they are neded.

$ mkdir -p client/js/test
```
