# mv
> move or rename a file or directory

`$ mv <source file path> <target file path>`  

Use `mv` to move a file or directory from one place to another on the filesystem. `mv` is also used to rename a file or directory.

## warning 
`mv` will overwrite an existing target file, and you can not get it back.

## important flags
* `-n` do not overwrite an existing file.
* `-v` cause move to be verbose, loging files as they are moved.

## examples 
``` sh 
# rename the file ./server.js to ./app.js

$ mv ./server.js ./app.js
```
``` sh
# move a the file ~/Downloads/jquery.min.js to the current directory

$ mv ~/.Downloads/jquery.min.js ./
```
``` sh
# move the directory ../assets to the current directory

$ mv ../assets ./
```
``` sh
# move the file ~/Desktop/screenshot.png to the current directory
# and rename it app_demo.png

mv ~/Desktop/screenshot.png ./app_demo.png
```
