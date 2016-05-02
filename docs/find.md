# find
> recursively search for files

`$ find <start directory> <flags> <options>`   
Use find to look for files by name, type, size, permissions, etc. Find generates a list of files that match a query. You can use this to help remember where a file is located. You can use the list generated from find with other programs.  

## important flags
* `-name` find files by their name
* `-iname` find files by their name **case insensitive**
* `-d` set the depth of directories to search

## examples
``` sh
# recursively find files of all .md files

$ find . -name '*.md'
```

``` sh
# find all files with the word readme

$ find . -iname '*rEaDMe*'
```

``` sh
# find all js files within 3 directories

$ find . -name '*.js' -d 3
```

``` sh
# open all the files with names that end with _test.js in vim

$ vim $(find . -name '*_test.js')
```
