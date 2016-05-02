# rm
> delete files and directories  

`$ cd <flags> <path>`  

`rm` will permanently remove a file or directory from your file system. Once you `rm` a file or directory you cannot get it back!

## warning
Be especially careful when you are removing a directory using, because everything in side it will be permanently deleted. If you run `rm -rf /` it will try to delete all of the files on your computer that have your user permissions!


## important flags
* `-rf` force a recursive delete of a directory

## examples

``` sh
# delete a file called data.csv.backup

$ rm data.csv.backup
```

``` sh
# delete a .git directory and all of its contents

rm -rf .git
```
