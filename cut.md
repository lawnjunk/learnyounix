# cut
> cut out selected portions of a line of text  

`$ cut <options> <optional filename>`   
Cut is used to grab specifc portions of a line of text. You can use cut to grab select portions of text from each line of a file, for example to print the second and fourth fileds from a **.csv** file. You can also use cut to filter portions of text from each line output by another program, for example selecting the list of file names from the output of `grep`.

## important flags
* `-d <delimter>`, `-f <fileds>` - set a delimiter to split each line by and which feilds to select
  * delimter is a string
  * feilds are a number, numbers seporated by `,`, or range of numbers seporated by `-`
* `-c` - select a character, characters seporated by `,`, or range of characters seporated by `-`

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
