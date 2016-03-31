# bash globs
> Pathname expansion

## pattern language
* `*` matches *any string* 
* `?` matches *any single character*
* `[]` defines a bracket epression  

**bracket expression**
* `[XYZ]` matches eather `X`, `Y`, or `Z`
* `[A-C]` matches the range of characters from `A` to `C`
* `[[:class:]]` matches all the characters in a [POSIX® character class](/character-class.md)
* `[^..]` nagating expression (matches everything but the expression)  

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
