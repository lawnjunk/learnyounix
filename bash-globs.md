# bash globs
> Pathname expansion  

Globs are a type of expression in bash that expands to list of files that match a PATTERN. You can use Globs to provide a list of files as the arguments to a program. Globs can also be used with loops in order to iterate over files.  

## pattern language
* `*` matches *any string* 
* `?` matches *any single character*
* `[]` defines a bracket epression  

**bracket expression**
* `[XYZ]` matches eather `X`, `Y`, or `Z`
* `[A-C]` matches the range of characters from `A` to `C`
* `[[:class:]]` matches all the characters in a [POSIX® character class](/character-class.md)
* `[^..]` nagating expression (matches everything but the expression)  

**extended pattern language**
> these will only work if the `extglob` shell option is turned on  

* a pattern list is one or more patterns seporated by the `|` character
 * `*.js|img/*-[0-9][0-9].png|**/*.html` matches all `.js` 
* `@(<pattern-list>)` matches **one** occurance of a given pattern
* `*(<pattern-list>)` matches **zero or more** occurance of a given pattern
* `!(<pattern-list>)` matches **anything except** occurance of the given patterns
* `?(<pattern-list>)` matches **zero or one**  of the given patterns
* `+(<pattern-list>)` matches **one or more** of a given pattern  

## customization
**enable and disable glob options**

* **enable** `shopt -s <option>` will enable an option  
* **disable** `shopt -u <option>` will disable an option  

**glob options**  

* `extglob` enable pattern list `*(txt|md|js)` 
* `dotglob` wildcard characters **can** match files begining with a `.`
* `globstar` the glob `**` will recursivly match files and directorys
* `nullglob` if no matches are found the glob will be replaced with and empty string
* `fialglob` if no matches are found an error will be produced
* `nocaseglob` case insensitive pathname expansion
* `globasciiranges` bracket ranges like `[A-Z]` use the _**C**_ locale rather than system locale

### disable all globs
``` sh
# to set a option in bash use 

$ set -f <option>
```

## examples
``` sh
# print a list of all the '.js` and css files in this directory

$ echo ./*.js
```
``` sh
# print a list of all files that are not '.html' files in the current directory

$ echo ./!(.html)
```
``` sh
# print a list of the files that are '.html' and '.css' files

$ echo ./*.(html|css)
```


