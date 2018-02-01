# supersonicscript
Ever wanted to add a brand new, freshly written bash script to your system?
Put it in /bin/ or ~/.local/bin, only to find you can't really manage it, and it gets lost among binaries?
Worry not!

mkscript "brand new $scriptname" will:
- create a script from a template in .script-template
- put it in a configurable $savepath/$scriptname
- put you straight into your $EDITOR
- check if file isn't empty, delete it if it is
- add an executable bit to your new script
- put a link to it at $linkpath/$scriptname, which hopefully is in your $PATH
- check for existence of $linkpath/$scriptname beforehand!

ALSO

mkscript "existing $scriptname" will:
- put you straight into you $EDITOR
- check if file isn't empty, delete it if it is
- TODO: make it unlink it when deleting the script

AND LAST BUT NOT LEAST

mkscript mkscript will:
- make a backup of itself
- proceed as normal
- ask you if you want to save or revert at the end of your $EDITOR session!

Never lose your ability to mkscript!
