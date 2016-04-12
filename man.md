# man
> display the manual for a command  

`$ man <command name>`  

Most built in programs have manual pages. The manual pages are usually organized by NAME, SYNOPSIS, DESCRIPTION, OTHER... The manual pages are usualy refered to as *man pages*. Man pages usually do not tell you when to use a program. They most often a reference what a program can do, and how to use a program. 

## usage
By default `man` uses the `less` pager to dispay files.
* to quit hit the leter `q`
* to search down the document hit `/` type your search string and hit `Enter`
* to search up the document hit `?` type your search string and hit `Enter`
* to cycle forward though search result hit the letter `n`
* to cycle backward though search result hit the letter `N`


## examples
``` sh
# get the manual for man

$ man man
```

``` sh
# get the manual for ls

$ man ls
```

