# pbcopy
> copies standard input to the clipboard
**This only works on osx**

Use `pbcopy` to copy the output of anoter command to the clipboard. It is usefult for copying error messages for searching on the internet, Or copying the output of a program to copy into your text-editor.

# examples
``` sh
# copy the contents of ~/.bashrc to the clipboard

$ cat ~/.bashrc | pbcopy
```
``` sh
# copy the output of pwd to the clipboard

$ pwd | pbcopy
```
