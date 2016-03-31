# cut
* using `cut` with a file
 * `$ cut <options> <filename>`  
* using cut with a pipe  
 * `<somer-command> | <cut> <options>`
* access indiviual fileds and chars with `,` seporated numbers 
* access field and char ranges with `-` seporated numbers  

## flags
* `-d <delimiter> -f <field>`  
``` sh
# cut stream by a ',' and print the second field

$ echo "one,two,three,four" | cut -d ',' -f 2,4`  
# two,four
```
* `-c` list 
``` sh
# print the first 8 characters 

$ echo "abcdefghijklmnopqrstuvwxyz" | cut -c 1-8
# abcdefgh
```
