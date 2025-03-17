# Git-GitHub Summary Tutorial

Git is a version control system that tracks changes in files such as code, text, and images. GitHub, on the other hand, is one of the remote repository platforms where projects can be stored and version-controlled using Git.

## 1. Installing Git

### 1a. Download Git
Download the appropriate Git version for your computer from the "Standalone Installer" section at this link: [Git Download](https://git-scm.com/downloads)

### 1b. Install Git
Proceed with the default installation settings. However, as a recommendation, you may choose the "Use OpenSSL library" option during installation.

### 1c. Configure Git with Username and Email
Set up Git with your user information:

```sh
git config --global user.name "yourusername"
git config --global user.email youraddress@xxmail.com
git config --list  # Check configured user details
```

## 2. Creating a Git Project
Navigate to the directory where your project files will be stored using the `cd` (change directory) command. Then initialize Git in that directory with the `git init` command. This creates a hidden `.git` folder and displays `(master)` in the terminal, indicating that Git is tracking the directory.

```sh
cd Desktop/yourpath
git init  # Initialize a Git repository in the current folder
```

## 3. Managing Files with Git

You can create folders and files in the working directory using Git commands:

```sh
mkdir yourdirectoryname  # Create a directory
touch yourfilename.xx    # Create a file
```
Alternatively, you can manually create files and folders using the right-click context menu.

Next, stage and commit the files to the local repository:

```sh
git add .  # Stage all files
git add example.txt  # Stage a specific file
git status  # Check the status of files
git commit -m "your commit message"  # Commit staged files to the local repository
```

Each time you modify or add new files, repeat the `git add` and `git commit` steps to update the local repository.

## 4. Pushing to GitHub

### 4a. Create a New Repository on GitHub
Go to GitHub, create a new repository, and enter a valid repository name. The repository name does not have to match your local folder name.

### 4b. Connect Local Repository to GitHub
Copy the repository link from the "Code" section in GitHub and link it to your local repository using the following command:

```sh
git remote add origin yourgithubrepolink
git remote  # Check the configured remote
```

Push the local repository to GitHub:

```sh
git push -u origin master  # Push to the master branch on GitHub
```

On the first push, you will be asked to authenticate in your browser. Select "Sign in with your browser," enter your GitHub credentials, and sign in.

Once completed, your files will be available in your GitHub repository.

## 5. Updating Data

If you modify files in your local repository, follow these steps to update them on GitHub:

```sh
git add .
git commit -m "Updated files"
git push  # Push the latest changes to GitHub
```

Now, your GitHub repository is updated!

## Notes

- For more details on Git, check out the official Git book: [Git Book](https://git-scm.com/book/en/v2)
- To customize your README file with formatting and images, refer to: [GitHub Formatting Guide](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- Explore GitHub README generator tools for enhanced customization.

Happy coding! 😊


