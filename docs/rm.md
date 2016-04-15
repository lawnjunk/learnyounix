# rm 
> delete files and directorys  

`$ cd <flags> <path>`  

`rm` will permanitly remove a file or directory from your filesystem. Once you `rm` a file or directory you cannot get it back! 

## warning
Be especially careful when you are removing a directory using, becuase everything in side it will be permanitly deleted. If you run `rm -rf /` it will try to delete all of the files on your computer that have your user permisions! 


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
