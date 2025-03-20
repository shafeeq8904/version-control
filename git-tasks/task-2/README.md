Created a .env File

The .env file is typically used to store environment variables such as API keys, database credentials, and other sensitive information.

# Create a .env file in your project directory
touch .env

Add the .env File to .gitignore

# Create a .gitignore file
$ touch .gitignore

Then, open .gitignore and add the following line:
.env
This ensures that the .env file will not be tracked by Git.

After setting up .gitignore, run the following command to check if .env is ignored:
 - git status
If the .env file does not appear in the list of untracked files, it means Git is correctly ignoring it.

git add .gitignore
git commit -m "Added .gitignore to exclude .env file"
git push origin main