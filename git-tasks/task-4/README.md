This guide demonstrates how to create, simulate, and resolve merge conflicts in Git by modifying the same file in two different branches.

# Create an index.html file
Created a basic structure in index.html
git add index.html
git commit -m "Initial commit with index.html"

# Create a New Branch
git checkout -b new-branch

# Switch back to main and modify index.html:
in this case modified the paragraph in index.html
git add index.html
git commit -m "Updated index.html in main"

# Modify index.html in new-branch
to develop a conflict modify the same line 
git add index.html
git commit -m "Updated index.html in new-branch"

# Now, switch to main and attempt to merge:
git checkout main
git merge new-branch
Since the same lines were modified in both branches, Git will raise a merge conflict.

# git status
Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   index.html

# Open the File and Resolve the Conflict
<<<<<<< HEAD
<p>Commit from main branch</p>
=======
<p>Commit from new-branch</p>
>>>>>>> new-branch
Manually edit the file to keep both changes or choose one:
Save the file after making changes.

# Mark Conflict as Resolved and Complete the Merge
git add index.html
git commit -m "Resolved merge conflict in index.html"

# To compare differences between branches before merging:
git diff main new-branch
