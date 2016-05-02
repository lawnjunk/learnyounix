# PS1
> the environment variable to configure your prompt

Changing the environment variable `$PS1` will change the what your prompt looks. There are special characters that enable you to add special information and color to your prompt. Setting your prompt to have the information you need at a glance can be very useful.

## bash special prompt escape characters
* `\h` hostname
* `\w` full path from home directory _(not recommended)_
* `\W` the current working directory _(recommended)_
* `\j` the number of background processes running spawned by this shell _(recommended for advanced users)_
* `\u` username
* `\l` the terminal name for the current shell

## color for the prompt
Ansi color codes for the terminal look like this `\[\033[01;32m\]`, that is the color green. Remembering color codes for the terminal is very hard, and not worth your time, so I made a snipped of code that sets variables for setting the color in your prompt. All you have to do to use these variables in your prompt is **copy this snippet before you set your PS1**. If your terminal does not support color, this snippet will default to no color.

``` sh
num_colors=$(tput colors)
if [ num_colors ];then
  txt_black="\[$(tput setaf 0)\]"   # black
  txt_red="\[$(tput setaf 1)\]"     # red
  txt_green="\[$(tput setaf 2)\]"   # green
  txt_yellow="\[$(tput setaf 3)\]"  # yellow
  txt_blue="\[$(tput setaf 4)\]"    # blue
  txt_magenta="\[$(tput setaf 5)\]" # magenta
  txt_cyan="\[$(tput setaf 6)\]"    # cyan
  txt_white="\[$(tput setaf 7)\]"   # white
  txt_reset="\[$(tput sgr0)\]"      # default
fi
```

Now all you not to do to change the color is use `$txt_red` or `$txt_cyan`

## examples
* place these in the bashrc file after the above color snippet
* make sure you are using double-quotes `"`

```sh
# set a basic prompt with no color 'username@hostname:current-directory $ '

export PS1="\u@\h:\W \$"
```
``` sh
# same as above but color code username and hostname
# cyan and current-directory magenta everything else white
# reset to default color at the end

export PS1="$txt_cyan\u$txt_white@$txt_cyan\h$txt_white:$txt_magenta\W $txt_white\$$txt_reset
```
