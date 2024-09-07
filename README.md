# **Installation and Setup Guide for the `gitbuddy` Script on Linux and macOS**
---

This guide will walk you through setting up and running the `gitbuddy` script, a handy tool designed to automate common Git tasks and streamline your workflow. With `gitbuddy`, you can easily manage Git operations like adding changes, committing, pulling, and pushing directly from your terminal. Additionally, the script integrates with ChatGPT to help generate commit messages and pull request descriptions.

### Introduction
`gitbuddy` is a Python-based script that simplifies your Git workflow by automating repetitive tasks. It allows you to perform actions like creating commits and interacting with remote repositories with ease. To enhance your productivity, `gitbuddy` also includes prompt templates for generating commit messages and pull requests using ChatGPT. These prompts are located in the `prompts` folder within the cloned repository and can be used to quickly generate high-quality messages by copying and pasting them into a blank ChatGPT chat.

### 1. **Clone the Repository with the `gitbuddy` Script**

First, clone the repository that contains the `gitbuddy` script. Make sure you have `git` installed on your system.

```bash
# Clone the repository
git clone https://github.com/JorgeSarricolea/git-buddy ~/Documents/scripts
```

> [!IMPORTANT]
Consider that a folder called `scripts` will be created that will be in `Documents`. This command will download the repository to the `~/Documents/scripts` folder.

### 2. **Make the Script Executable**

Once the script is cloned, navigate to the folder where the repository was downloaded and make the script executable.

```bash
cd ~/Documents/scripts
chmod +x gitbuddy
```

This command ensures that the `gitbuddy` script is executable.

### 3. **Add the Script to the `PATH`**

To run the script from anywhere by simply typing `gitbuddy`, you need to add the folder where the script is located to your system’s `PATH`.

- Edit your shell configuration file (`~/.bashrc`, `~/.bash_profile`, or `~/.zshrc`, depending on your system).

```bash
# For bash
nano ~/.bashrc
# For zsh
nano ~/.zshrc
```

- Add the following line at the end of the file:

```bash
export PATH="$HOME/Documents/scripts:$PATH"
```

- Save the file and reload it:

```bash
# Reload the file
source ~/.bashrc  # For bash
source ~/.zshrc   # For zsh
```

Now you can run `gitbuddy` from any directory.

### 4. **Install Python (if needed)**

Make sure you have Python 3 installed, as the script depends on it. Check the Python version on your system:

```bash
python3 --version
```

If you don't have Python 3, you can install it:

- **On Linux (Ubuntu/Debian)**:

```bash
sudo apt update
sudo apt install python3
```

- **On macOS**:

```bash
brew install python3
```

### 5. **Test the Script**

After setting everything up, you can test the script.

- Navigate to any Git repository on your machine:

```bash
cd /path/to/your/repo
```

- Run the script by typing `gitbuddy`:

```bash
gitbuddy
```

The script will guide you through the process of adding changes, creating a commit with a custom message, and performing `push` or `pull` actions as needed.

---

By following these steps, you’ll have successfully set up and run the `gitbuddy` script on your Linux or macOS system. You can now use it from anywhere in your terminal to streamline your Git workflow!