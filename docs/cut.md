# cut
> cut out selected portions of a line of text  

`$ cut <options> <optional filename>`   
Cut is used to grab specific portions of a line of text. You can use cut to grab select portions of text from each line of a file, for example to print the second and fourth files from a **.csv** file. You can also use cut to filter portions of text from each line output by another program, for example selecting the list of file names from the output of `grep`.

## important flags
* `-d <delimter>`, `-f <fileds>` - set a delimiter to split each line by and which fields to select
  * delimiter is a string
  * fields are a number, numbers separated by `,`, or range of numbers separated by `-`
* `-c` - select a character, characters separated by `,`, or range of characters separated by `-`

## examples
``` sh
# cut stream by a ',' and print the second field

$ echo "one,two,three,four" | cut -d ',' -f 2,4`  
# two,four
```

``` sh
# print the first 8 characters

$ echo "abcdefghijklmnopqrstuvwxyz" | cut -c 1-8
# abcdefgh
```
