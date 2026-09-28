# Card Log (Partner A)

##Card 1
Commit had a bad message. Fix: git commit --amend. Helped edit the original commit to a new one.

##Card 2
The file "notes.txt" was never meant to be listed under "Changes to be committed". 
git restore --staged notes.txt helped untrack the notes file and rm helped remove the notes file.

##Card 3
The fake password was in the local history, but it has not been pushed.
"git reset --soft...", "git reset...", and "git reset --hard". --soft moved the branch pointer 
to the targeted commit, but leaves both in the staging area and the working directory. No flag 
moves the branch pointer back and resets the staging area. -hard moves the branch pointer, resets
the staging area and overwrites the working directory.

##Card 4

Cargo build failed and the false commit was sent to GitHub. "git revert HEAD" helped undo the 
original commit and creates a new one, incase for any teammates who already pulled.
