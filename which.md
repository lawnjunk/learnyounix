# which
> locate a command in the `$PATH` variable  

`$ which <flags> <command name>`   

The `which` command will tell you where a command is in the `$PATH` variable. By defualt the which command will tell you the first path to the command found in the `$PATH` variable from left to right. The first command found from left to right is the command that will run when you you type that commands name.

## flags
* `-a` list all instances of executables found (instead of just the first one)

## examples
``` sh
# print the path to the 'ls' command

$ which ls
```
``` sh
# print the paths to all the vim commands found in '$PATH'

$ which -a vim
```
