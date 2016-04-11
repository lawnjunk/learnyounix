# grep
> search lines for a matching regular expression  
`grep <flags> <search term> <optional file paths>`

Grep is used to search lines for a matching regular expression. You can use it to search files for occurances of a pattern, for example look for the file that that defines a class. You can use it to fitler the output of another program, for example to print all of the lines with the PATTERN `'inet'` from `ifconfig`. Grep prints out the lines that match a PATTERN, and the filename if any.

## important flags
* `-i` ignore case
* `-r` recursivly
* `-n` show line numbers
* `-E` regular expression
* `-v` invert match (seleced lines are those **not** matching the pattern)
* `-w` look for entire pattern intact
* `-c` count occurances

## examples
``` sh
# search a direcory for a files that contain the PATTERN 'class Admin('

$ grep 'class Admin(' ./*
```
``` sh
# filter the output of ifconfig to print my local ip but not loopback
# left space after 'inet' so that 'inet6' gets filtered out

$ ifconfig |grep 'inet ' |  grep -v '127.0.0.1'
```


