# tree
> list contents of directorys in a tree like format  

`$ tree <flags> <optional dirname>`  
Tree is a recursive directory listing program that prints an easy to read list of directorys and files. It is a better way to recursivly see the content of a directory than `$ ls -R`

## important flags
* `-L <number>` max level of depth to traverse
* `-d` directories only
* `-P <PATTERN>` list only files that match the wildcard PATTERN
* `-I <PATTERN>` dont list the files that match the wilde card pattern

## examples
``` sh
# recursivly print a tree of the current working directory

$ tree
```

``` sh
# recursivly print a tree of the cleint/js directoy but only go 2 levels deep

$ tree -L 2 client/js
```
``` sh
# recursivly print a tree of the current working directory but ignore
# the node_modules directory

$ tree -I node_modules
```
