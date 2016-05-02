# ls
> list contents of current working directory  

`$ ls <flags> <optional dirname>`  

Use `ls` to list the names and information about the contents of the current working directory.

## flags
* `-a` also list hidden files (files whose names start with`.`)
* `-l` also list the permissions, owner, group, size, and time-last-modified
* `-h` make the `-l` flag list the file size in human readable form (bytes, kilobytes)

### color osx
* `-G` make ls color coded by file type

### color linux
* `--color=auto` make ls color coded by file type

## examples
``` sh
# print list of files in current directory color coded by file type

$ ls -G
```

``` sh
# print list of all files (including hidden) in current directory color coded by file type

$ ls -aG
```

``` sh
# print list of all files and human readable info color coded by file type

$ ls -lahG
```

``` sh
# print list of files in the directory '~/Downloads' color coded by file type

$ ls -G ~/Downloads
```
