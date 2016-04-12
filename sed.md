# sed
> edit lines of text  

`$ sed <flags> <expression> <optional filename>`  
Sed is used to edit lines of text. It can be used to search and replace PATTERNS with a string, or delete PATTERNS. Sed can edit files in place, for example if you wanted to rename all the ocurrences of a variable in a list of javascript files. Sed can also edit streams of output from other commands.

## important flags
* `-e` allows you to apply sed to a stream of text
* `i` allows you to apply sed to a file inplace

## sed patterns
* `s/<search PATTERN>/<replace string>/` search and repalce
* `/<search PATTERN>/d` seach and delete
* `s/<search PATTERN>/<replace string>/g` without the `/g` flag sed will only effect the first matched PATTERN in each line

## examples
 * `sed -e <sed PATTERN>`
``` sh
# Replace all ',' with ' ' from a stream

$ echo "hello,world" | sed -e 's/,/ /g'
# hello world
```
``` sh
# Replace all occurances of getName with getUserName for all .js 
# files in the current working directory, & don't create backup files

$ sed -i '' 's/getName/getUserName/g' *.js
```
