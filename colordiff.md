# colordiff
* `-u` output 3 lines of unified context
 * _looks like a git diff_
``` sh
$ colordiff -u file1 file2
```

* `-y` get output with side by side output
``` sh
$ colordiff -y file1 file2
```

* *add line numbers with* **cat**
``` sh
$ colordif -y <(cat -n file1) <(cat -n file2)
```
