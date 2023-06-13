shell variables expansion
alias ls="rm *"
echo hello $USER
export PATH=$PATH:/action
echo $((`echo $PATH | grep -o ":/" | wc -1` + 1))
printenv
