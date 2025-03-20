This document guides you through initializing a Git repository, making commits, creating a branch, and merging it back into the main branch.

# Navigate to your project folder

# Initialize Git
git init

# Create an index.html file
Created a basic structure in index.html

# Add the file to the staging area
git add index.html

# Commit the changes
git commit -m "Added index.html in the main branch"

# Create a new branch named nav-bar
git branch nav-bar

# Switch to the nav-bar branch
git checkout nav-bar

# Create a nav-bar.html file
Created a basic structure in nav-bar.html

# Add and commit the file
git add nav-bar.html
git commit -m "Added nav-bar.html in the nav-bar branch"

# Switch back to the main branch
git checkout main

# Merge the nav-bar branch into main
git merge nav-bar

# Add a remote repository
git remote add origin <repository-url>

# Push the main branch to GitHub
git push -u origin main