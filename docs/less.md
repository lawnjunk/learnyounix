# less
> page through file contents  

`$ less <filename>`

Less is used to read and search though files and output streams. Often it is used in place of `cat` to read long files because it has the ability to scroll up and down.

## usage
* to quit hit the letter `q`
* to search down the document hit `/` type your search string and hit `Enter`
* to search up the document hit `?` type your search string and hit `Enter`
* to cycle forward though search result hit the letter `n`
* to cycle backward though search result hit the letter `N`

## examples
``` sh
# read a file called app.js

$ less app.js
```

``` sh
# read the output of curls --help in less

$ curl --help | less
```
