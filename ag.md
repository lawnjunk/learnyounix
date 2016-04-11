# ag
> recursivly search for files by their content
  
`$ find <regular expression> <optional file/dir name>`  
Use ag to look for files by their contents. Find can help you figure out where you declared a method, and/or all the places you have used a method. You can use the output of find with other programs.  

## important flags
* `-a` seach dot files too
* `-i` ignore case
* `-v` invert match 
* `-w` look for entire pattern intact
* `--depth` set the directory depth 
* `-c` count the number of matches
* `-f` follow symlinks

# examples
``` sh
# recursivly find lines with a string & print line numbers

$ ag 'imageDataObject'
```

``` sh
# search a file for the PATTERN document.createElement

$ ag 'document.createElement'
```

``` sh
# look for the string 'table' in .js and .html files

$ ag 'table' --js --html
```

``` sh
# get a list of all the files containing the PATTERN document in thier contents

ag 'document' |cut -d ':' -f 1 | uniq
```
