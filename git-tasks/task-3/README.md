git restore is used to undo changes in your working directory before staging them. If you've modified a file but haven’t added it to staging, running git restore <file> will discard those changes and return the file to its last committed state.

git reset works at different levels. When used with git reset <file>, it unstages a file that was added to the staging area but doesn’t remove changes from your working directory. 

git revert is the safest way to undo a commit because instead of erasing history, it creates a new commit that negates the effects of a previous commit. This keeps the history intact and is the recommended approach when working in shared repositories.
