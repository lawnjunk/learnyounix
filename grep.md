# grep
* using grep with a file or list of files
 * `grep <flags> <search term> <file paths>`
* using grep with a pipe
 * `<some command> | grep <flags> <search term>`
## flags
* `-i` ignore case
* `-r` recursivly
* `-n` show line numbers
* `-E` regular expression
* `-v` invert match (seleced lines are those **not** matching the pattern)
* `-w` look for entire pattern intact
* `-c` count occurances
