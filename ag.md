# ag
> recursivly search for files by their content
  
`$ ag <regular expression> <optional file/dir name>`  
Use ag to look for files by their contents. `ag` can help you figure out where you declared a method, and/or all the places you have used a method. You can use the output of `ag` with other programs. By default `ag` prints a list of all the files that match a query with numbered occurances of the lines that match the query.

## important flags
* `-a` seach dot files too
* `-i` ignore case
* `-v` invert match 
* `-w` look for entire pattern intact
* `--depth` set the directory depth 
* `-c` count the number of matches
* `-f` follow symlinks

## examples
``` sh
# recursivly find lines with the PATTERN 'imageDataObject' 

$ ag 'imageDataObject'
```

``` sh
# search for the PATTERN document.createElement in the client/js directory

$ ag 'document.createElement' client/js
```

``` sh
# look for the PATTERN 'table' in .js and .html files

$ ag 'table' --js --html
```

``` sh
# get a list of all the files containing the PATTERN 'document' in thier contents

ag 'document' |cut -d ':' -f 1 | uniq
```
