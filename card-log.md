# Card Log (Partner B)

## Card 1
Commit had a bad message -> git commit --amend -> helped replace the last commit instead of adding a 
new one

## Card 2
The file "notes.txt" was under "Changes to be commited", but never meant to commit it -> "git
restore -- staged notes.txt" then "rm notes.txt" -> The first one unstages it without deleting it
so is is untracked again, then the next one removes it.
