# find
> recursivly search for files

`$ find <start directory> <flags> <options>`   
Use find to look for files by name, type, size, permissions, ect. Find genorates a list of files that match a query. You can use this to help remember where a file is located. You can use the list genorated from find with other programs.  

## important flags
* `-name` find files by their name
* `-iname` find files by ther name **case insensitive**
* `-d` set the depth of directorys to search

# examples
``` sh
# recursivly find files of all .md files
 
$ find . -name '*.md'
```

``` sh
# find all files with the word readme

$ find . -iname '*rEaDMe*'
```

``` sh
# find all js files within 3 directorys

$ find . -name '*.js' -d 3
```

``` sh
# open all the files with names that end with _test.js in vim

$ vim $(find . -name '*_test.js')
```
