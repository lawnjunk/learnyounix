# sed
* sed `/g` pattern flag
 * place pattern flags at the end of a sed pattern
 * without the `/g` flag sed will only effect the first matched string in each line
* `-e` allows you to apply sed to a pipe 
 * `sed -e <sed pattern>`
``` sh
# Replace all ',' with ' ' from a pipe

$ echo "hello,world" | sed -e 's/,/ /g'
# hello world
```
* `-i` allows you to apply sed to a list of files in-place
 * `sed -i <backup extenstion> <sed pattern> file`
``` sh
# Replace all occurances of getName with getUserName for all .js 
files in the current working directory, & don't create backup files

$ sed -i '' 's/getName/getUserName/g' *.js
```
