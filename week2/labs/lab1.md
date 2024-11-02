# Step-by-Step Git Lab with Explanations

## Step 1: Create a New Repository in a Folder

```bash
mkdir my_project  # Create a new directory for your project
cd my_project     # Navigate into the project folder
git init          # Initialize a new Git repository in this folder
```

**Explanation**: The `git init` command initializes a new Git repository in the specified folder, allowing you to start tracking changes in your project files.

## Step 2: Configure Git Username and Email

```bash
git config --global user.name "Your Name"       # Set the global Git username
git config --global user.email "your@email.com"  # Set the global Git email address
```

**Explanation**: These commands configure your Git identity, which will be associated with all your commits. This helps track changes and identify who made specific modifications in a collaborative environment.

## Step 3: Add the First Commit

```bash
touch README.md                # Create a new README file
git add README.md              # Stage the README file for commit
git commit -m "Initial commit" # Commit the staged file with a message
```

**Explanation**: The `touch` command creates a new README file. The `git add` command stages the file, making it ready to be committed. Finally, `git commit` permanently records the changes in the repository with a descriptive message.

## Step 4: Modify the File and Commit the Changes

```bash
echo 'Project description' >> README.md  # Modify the README file by adding a project description
git add README.md                        # Stage the modified file for commit
git commit -m "Update README with project description"  # Commit the changes with a descriptive message
```

**Explanation**: The `echo` command appends text to the README file, modifying it. The `git add` command stages the changes for the next commit, and `git commit` records the new changes in the repository.

## Step 5: Roll Back Changes

```bash
git log                         # View the commit history to identify the commit hash
git revert <commit-hash>        # Revert the specified commit, creating a new commit that undoes the changes
git reset --hard <commit-hash>  # Alternatively, reset to a previous commit (warning: can lead to data loss)
```

**Explanation**: The `git log` command helps you view the commit history and identify the commit you want to revert. The `git revert` command creates a new commit that undoes the changes while preserving the history. The `git reset --hard` command can also roll back changes to a specific commit, but it should be used with caution as it can permanently discard changes.

## Step 6: Secure the Local Code with Pre-Commit Hooks

```bash
# Install the pre-commit tool
pip install pre-commit  # Install the pre-commit tool globally

# Create a configuration file for pre-commit
# Step-by-Step Git Lab with Explanations

## Step 1: Create a New Repository in a Folder

```bash
mkdir my_project  # Create a new directory for your project
cd my_project     # Navigate into the project folder
git init          # Initialize a new Git repository in this folder
```

**Explanation**: The `git init` command initializes a new Git repository in the specified folder, allowing you to start tracking changes in your project files.

## Step 2: Configure Git Username and Email

```bash
git config --global user.name "Your Name"       # Set the global Git username
git config --global user.email "your@email.com"  # Set the global Git email address
```

**Explanation**: These commands configure your Git identity, which will be associated with all your commits. This helps track changes and identify who made specific modifications in a collaborative environment.

## Step 3: Add the First Commit

```bash
touch README.md                # Create a new README file
git add README.md              # Stage the README file for commit
git commit -m "Initial commit" # Commit the staged file with a message
```

**Explanation**: The `touch` command creates a new README file. The `git add` command stages the file, making it ready to be committed. Finally, `git commit` permanently records the changes in the repository with a descriptive message.

## Step 4: Modify the File and Commit the Changes

```bash
echo 'Project description' >> README.md  # Modify the README file by adding a project description
git add README.md                        # Stage the modified file for commit
git commit -m "Update README with project description"  # Commit the changes with a descriptive message
```

**Explanation**: The `echo` command appends text to the README file, modifying it. The `git add` command stages the changes for the next commit, and `git commit` records the new changes in the repository.

## Step 5: Roll Back Changes

```bash
git log                         # View the commit history to identify the commit hash
git revert <commit-hash>        # Revert the specified commit, creating a new commit that undoes the changes
git reset --hard <commit-hash>  # Alternatively, reset to a previous commit (warning: can lead to data loss)
```

**Explanation**: The `git log` command helps you view the commit history and identify the commit you want to revert. The `git revert` command creates a new commit that undoes the changes while preserving the history. The `git reset --hard` command can also roll back changes to a specific commit, but it should be used with caution as it can permanently discard changes.

## Step 6: Secure the Local Code with Pre-Commit Hooks

```bash
# Install the pre-commit tool
pip install pre-commit  # Install the pre-commit tool globally

# Create a configuration file for pre-commit
cat <<EOL > .pre-commit-config.yaml
repos:
  - repo: https://github.com/pre-commit/pre-commit-hooks
    rev: v4.0.1
    hooks:
      - id: trailing-whitespace
      - id: end-of-file-fixer
      - id: check-yaml
EOL  # Generate a sample pre-commit configuration file

# Install the hooks defined in the configuration
pre-commit install  # Install pre-commit hooks in the local repository
```

**Explanation**: Pre-commit hooks are scripts that run automatically before you make a commit. These hooks help catch issues early in the development process, such as formatting errors or other coding standard violations. By using pre-commit hooks, you can enforce coding standards and ensure higher code quality in your repository.

# Step-by-Step Git Lab with Explanations

## Step 1: Create a New Repository in a Folder

```bash
mkdir my_project  # Create a new directory for your project
cd my_project     # Navigate into the project folder
git init          # Initialize a new Git repository in this folder
```

**Explanation**: The `git init` command initializes a new Git repository in the specified folder, allowing you to start tracking changes in your project files.

## Step 2: Configure Git Username and Email

```bash
git config --global user.name "Your Name"       # Set the global Git username
git config --global user.email "your@email.com"  # Set the global Git email address
```

**Explanation**: These commands configure your Git identity, which will be associated with all your commits. This helps track changes and identify who made specific modifications in a collaborative environment.

## Step 3: Add the First Commit

```bash
touch README.md                # Create a new README file
git add README.md              # Stage the README file for commit
git commit -m "Initial commit" # Commit the staged file with a message
```

**Explanation**: The `touch` command creates a new README file. The `git add` command stages the file, making it ready to be committed. Finally, `git commit` permanently records the changes in the repository with a descriptive message.

## Step 4: Modify the File and Commit the Changes

```bash
echo 'Project description' >> README.md  # Modify the README file by adding a project description
git add README.md                        # Stage the modified file for commit
git commit -m "Update README with project description"  # Commit the changes with a descriptive message


```

**Explanation**: The `echo` command appends text to the README file, modifying it. The `git add` command stages the changes for the next commit, and `git commit` records the new changes in the repository.

## Step 5: Roll Back Changes

```bash
git log                         # View the commit history to identify the commit hash
git revert <commit-hash>        # Revert the specified commit, creating a new commit that undoes the changes
git reset --hard <commit-hash>  # Alternatively, reset to a previous commit (warning: can lead to data loss)
```

**Explanation**: The `git log` command helps you view the commit history and identify the commit you want to revert. The `git revert` command creates a new commit that undoes the changes while preserving the history. The `git reset --hard` command can also roll back changes to a specific commit, but it should be used with caution as it can permanently discard changes.

## Step 6: Secure the Local Code with Pre-Commit Hooks

```bash
# Install the pre-commit tool
pip install pre-commit  # Install the pre-commit tool globally

# Create a configuration file for pre-commit
cat <<EOL > .pre-commit-config.yaml
repos:
  - repo: https://github.com/pre-commit/pre-commit-hooks
    rev: v4.0.1
    hooks:
      - id: trailing-whitespace
      - id: end-of-file-fixer
      - id: check-yaml
EOL  # Generate a sample pre-commit configuration file

# Install the hooks defined in the configuration
pre-commit install  # Install pre-commit hooks in the local repository
```

**Explanation**: Pre-commit hooks are scripts that run automatically before you make a commit. These hooks help catch issues early in the development process, such as formatting errors or other coding standard violations. By using pre-commit hooks, you can enforce coding standards and ensure higher code quality in your repository.

## Step 7: Add Another Commit and See Pre-Commit in Action

```bash
echo 'Additional project details' >> README.md  # Modify the README file again
git add README.md                              # Stage the changes
git commit -m "Add more details to README"       # Commit the changes and see pre-commit hooks in action
```

**Explanation**: In this step, we modify the README file again and commit the changes. When running `git commit`, the pre-commit hooks will automatically execute, checking for issues like trailing whitespace or formatting errors. If any issues are detected, they must be fixed before the commit can proceed.
