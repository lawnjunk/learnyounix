# colordiff
> compare files line by line  

`colordiff <flags> <file one> <file two>`  

Colordiff will compare two files line by line and tell you how they differ. You can use it to compare to source files and see if their contents differ.

# important flags
* `-u` output 3 lines of unified context
* `-y` get output with side by side output

# examples
``` sh
# print the lines of a file that differ and
# the three lines above and below for context

$ colordiff -u file1 file2
```
``` sh
# print out two files side by side and color-code their differences

$ colordiff -y file1 file2
```
``` sh
# colordiff side by side but add line numbers to files

$ colordiff -y <(cat -n file1) <(cat -n file2)
```
