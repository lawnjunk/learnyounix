# $PATH
> environment variable that sets where executable programs are located   

The `$PATH` variable sets a list of directorys where executable programs live. All of the comands you use live in one of these directorys. If you have an executable file you want to run by typing its name you can put it in one of the directorys found in `$PATH`. The order of the directorys in `$PATH` is very imortant. The first command found in the `$PATH` directorys from left to right is the command that will run when you you type that commands name. It is possible for their to be more than one version of a command on your machine, but only one will run. You can add directorys to `$PATH` to enable your `shell` to look in anoter directoy. If you set the `$PATH` variable to an empty string, the only way you can run programs is by typing their absolute path. It is a good idea to create your own **~/.bin** directory, and add it to `$PATH`. Then you dont have to mix your programs into the systems directorys.  

## reading the $PATH variable
In bash directorys in the `$PATH` are seporated by a colon `:`  
`/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin `

## adding a directory to $PATH
``` sh
# add the directory ~/.bin to the beginning of $PATH
# putting ~/.bin first means that any program in it will
# run instead of another program with the same name in the
# system directorys

export PATH="$HOME/.bin:$PATH"
```
