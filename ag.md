# ag
* recursivly search for a PATTERN in a PATH
``` sh
# recursivly find lines with a string & print line numbers
# with color coded output

$ ag 'imageDataObject'
```

* search a specific file for a PATTERN
``` sh
# search a file for the PATTERN document.createElement

$ ag 'document.createElement'
```
* recursilvy search for a PATERN in html and js files
 * `--<file-extenstion>` limit the files searched by `.<file-extnesion`
``` sh
# look for the string 'table' in .js and .html files

$ ag 'table' --js --html
```

## flags
* `-a` seach dot files too
* `-i` ignore case
* `-v` invert match 
* `-w` look for entire pattern intact
* `--depth` set the directory depth 
* `-c` count the number of matches
* `-f` follow symlinks

# tricks
``` sh
# get a list of all the files containing the PATTERN document in thier contents

ag 'document' |cut -d ':' -f 1 | uniq
```
