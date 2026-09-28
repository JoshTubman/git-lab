# Card Log (Partner B)

## Card 1
Commit had a bad message -> git commit --amend -> helped replace the last commit instead of adding a 
new one

## Card 2
The file "notes.txt" was under "Changes to be commited", but never meant to commit it -> "git
restore -- staged notes.txt" then "rm notes.txt" -> The first one unstages it without deleting it
so is is untracked again, then the next one removes it.

## Card 3
The fake password was in the local history, but has not been pushed -> "git reset --soft...",
"git reset...", "git reset -- hard" -> --soft moves branch pointer mack to the target commit, but
leaves both the staging area and the working directory untouched. No flag moves the branch pointer
back and resets the staging area, but leaves the working directory alone. --hard moves the branch 
pointer, resets the staging area, and overwrites the working directory to match the target commit.

## Card 4
Cargo build fails and the broken commit is now on GitHub -> "git revert HEAD" -> creates a new
commit that undoes an old one so that it is safe for those who may already have pulled it.
