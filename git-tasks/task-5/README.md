This guide demonstrates how to use Git interactive rebase to clean up commit history by squashing, reordering, and editing commits before merging into the main branch.

#  Create index.html
git add index.html
git commit -m "Initial commit"

# Make a Series of Commits
git add index.html
git commit -m "nav bar added"

git add index.html
git commit -m "Fix typo in fotter"

git add index.html
git commit -m "update rebase desc"

# To check the commit history:
git log --oneline

# To check the commit history:
git rebase -i HEAD~n
in this case i selected n as 3

# This will open a text editor showing recent commits:
pick 1a2b3c4 nav bar added
squash 2d3e4f5 Fix typo in fotter
squash 3f4g5h6 update rebase desc

squash - Merge the commit with the previous one.

# After saving, Git prompts you to edit commit messages:
combination of three commits

