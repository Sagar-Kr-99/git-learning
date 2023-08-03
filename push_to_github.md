```

#!/bin/bash


# Replace the following commands with your desired changes or commits
# For example:
# git add .
# git commit -m "Your commit message"
# git push origin main

# Change to your project directory
#cd /path/to/your/project
cd .
# Initialize a new Git repository (if it's not already initialized)
#git init

# Check if the .git directory already exists (repository already initialized)
if [ -d ".git" ]; then
  echo "Git repository already initialized. Skipping 'git init'."
else
  # If .git directory does not exist, initialize a new Git repository
  git init
fi
echo "init steps complete"
# Add all changes to the staging area
git add .
echo "add complete"

# Commit the changes with a commit message
git commit -m "Your commit message"

echo "commit complete"
# Set the remote repository URL
#git remote add origin "$REPO_URL"
# Check if the remote named "origin" already exists

if git remote get-url origin >/dev/null 2>&1; then
  # If "origin" already exists, update the remote URL
  git remote set-url origin "$REPO_URL"
else
  # If "origin" does not exist, add the new remote repository
  git remote add origin "$REPO_URL"
fi
echo "setting url"
# Authenticate with GitHub using the provided username and password/token
# Note: It's better to use an access token rather than a password for security reasons
# If you're using a token, make sure it has the necessary permissions to push to the repository.
# To create a token, go to: https://github.com/settings/tokens
# And then set it as an environment variable or pass it directly here.
git config credential.helper store <<<"url=https://$USERNAME:$PASSWORD@$REPO_URL"

# Push changes to the specified branch (e.g., main)
git push origin "$BRANCH"

# Clean up credentials after pushing
git config --unset credential.helper

echo "Changes pushed to GitHub successfully!"

```
