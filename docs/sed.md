# sed
> edit lines of text  

`$ sed <flags> <expression> <optional filename>`  
Sed is used to edit lines of text. It can be used to search and replace PATTERNS with a string, or delete PATTERNS. Sed can edit files in place, for example if you wanted to rename all the occurrences of a variable in a list of JavaScript files. Sed can also edit streams of output from other commands.

## important flags
* `-e` allows you to apply sed to a stream of text
* `-i` allows you to apply sed to a file in place

## sed patterns
* `s/<search PATTERN>/<replace string>/` search and replace first matched PATTERN in each line
* `/<search PATTERN>/d` search and delete  first matched PATTERN in each line
* `<sed expression>/g` use `/g` apply sed expression to all matched PATTERNs in each line

## examples
``` sh
# Replace all ',' with ' ' from a stream

$ echo "hello,world" | sed -e 's/,/ /g'
```
``` sh
# Replace all occurrences of getName with getUserName for all '.js'
# files in the current working directory

$ sed -i '' 's/getName/getUserName/g' *.js
```
