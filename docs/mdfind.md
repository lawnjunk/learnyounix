# mdfind
> spotlight for the commandline
**This only works on OS X**

`$ mdfind <flags> <query string>`

osx collects the metadata from all your files and mdfind lets you search through that metadata. This is what spotlight does behind the curtain.

## examples
``` sh
# search for files with the string 'mp4' in their metadata

$ mdfind mp4
```

``` sh
# search for files with the name 'grep.md'

$ find -name grep.md
```


