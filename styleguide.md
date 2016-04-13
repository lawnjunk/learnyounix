file names: `**filename**` -> **unicorn.md**  
file extension: `**.ext**` -> **.md**  
literal string: `'string'` -> `'**/*.js'`  
inline command: `command` ->  `grep`


comand description: `$ command` -> `$ ls`  
argument description: `<argument description>` -> `$ ls <flag>`  
optional argument: `<optional argument description>` -> `$ ag ... <optional file/dir name>`  

examples
```
> ``` sh
> # description of what you are going to accomplish
> $ command <arg1> <arg2>
> ``` 
```
->
``` sh
# use grep to filter history for the occurences of the word 'curl'

$ history |grep 'curl'
```

