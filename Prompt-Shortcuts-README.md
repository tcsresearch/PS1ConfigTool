You could build upon @goldilocks and @Michael Durrant's answers to create something more readable like this:

```
CYAN="\[\e[01;36m\]"
WHITE="\[\e[01;37m\]"
BLUE="\[\e[01;34m\]"
TEXT_RESET="\[\e[00m\]"   
TIME="\t"
CURRENT_PATH="\W"
ROOT_OR_NOT="\$"
```

Here is an example of the new PS1 code for the $PS1Select_* profiles: <br>
```export PS1="${CYAN}[${BLUE}${TIME}${WHITE} ${CURRENT_PATH}${CYAN}]${ROOT_OR_NOT}${TEXT_RESET} "```
