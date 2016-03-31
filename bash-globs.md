# bash globs
> Pathname expansion


## Customization

**enable and disable glob options**

* **enable** `shopt -s <option>` will enable an option  
* **disable** `shopt -u <option>` will disable an option  

**glob options**  

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
