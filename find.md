# find
* `$ find <start directory> <flags> <options>`
## flags
* `-name` find files by their name
``` sh
# recursivly find files of all .md files
 
$ find . -name '*.md'
```
* `iname` find files by ther name **case insensitive**
``` sh
# find all files with the word readme

$ find . -iname '*rEaDMe*'
```
* `-d` set the depth
``` sh
# find all js files within 3 directorys

$ find . -name '*.js' -d 3
```
