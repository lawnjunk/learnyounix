# cat 
> print file contents  

`$ cat <flags> <filename list>`

`cat` will print the contents of a file. Cats name comes from concatenate. It is often used to print multiple files at a singe time.

## important flags
* -n number the output lines

## examples
``` sh
# print the contents of help.md and man.md

$ cat help.md man.md
```

``` sh
# print the contents of ~/.bashrc with line numbers

$ cat -n ~/.bash_profile
```
