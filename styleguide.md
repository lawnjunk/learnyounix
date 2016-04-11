file names: `**filename**` -> **unicorn.md**  
file extension: `**.ext**` -> **.md**  
literal string: `'string'` -> `'**/*.js'`  
inline command: `command` ->  `grep`


comand description: `$ command` -> `$ ls`  
arument description: `<arument description>` -> `$ ls <flag>`  
optional arument: `<optional arument description>` -> `$ ag ... <optional file/dir name>`  

examples
```
> ``` sh
> # description of what you are going to acomplish
> $ command <arg1> <arg2>
> ``` 
```
->
``` sh
# use grep to filter history for the ocurances of the workd 'curl'

$ history |grep 'curl'
```

