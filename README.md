# GitAutoPush

![Project Image](https://github.com/muhfalihr/mystorage/blob/master/20240508_161828.png)

### Description

**GitAutoPush** is a user-friendly Bash script designed to automate the process of adding, committing, and pushing changes to a Git repository. With a clean and interactive command-line interface, this script simplifies version control operations and enhances productivity.

### Features

- **Loading Spinner**: Displays a spinner animation during the `git add` process to indicate ongoing operations.
- **Commit Prompt**: Prompts the user to enter a commit message interactively.
- **Environment Variable Display**: Shows the `GITHUB_ACCESS_TOKEN` for convenience.
- **Error Handling**: Checks for the existence of a `.git` directory and handles errors gracefully.
- **Customizable Separators**: Uses dynamic separators with titles for organized output.

### Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/muhfalihr/GitAutoPush.git
   cd GitAutoPush
   ```

2. **Make the Script Executable**:
   ```bash
   chmod +x gitautopush.sh
   ```

3. Add the directory location of the gitautopush file to the `PATH` environment variable Create an environment variable for `GITHUB_ACCESS_TOKEN` in the files `~/.bashrc` ( **for bash shell** ), `~/.zshrc` ( **for zsh shell** ), `~/.config/fish/config.fish` ( **for fish shell** ). Because I use the ***zsh shell***, for this practice I edited the configuration in the `~/.zshrc` file.

    ```bash
    nano ~/.zshrc
    ```

    Add the **gitautopush directory** to the `PATH` environment variable

    ```bash
    export GITHUB_ACCESS_TOKEN=<github-access-token>
    export PATH=$PATH:/path/to/GitAutoPush
    ```

    save changes to the `~/.zshrc` file

4. Set environment variables

    ```bash
    source ~/.zshrc
    ```

5. **Run the Script**:
   ```bash
   gitautopush.sh
   ```

### Prerequisites

- Ensure that you have Git installed on your system.
- Make sure you are in the root directory of a Git repository before running the script.

### Requirements

1. Install figlet

    ```sh
    apt install figlet
    ```

### Example Output

```sh
↳ Enter a message to commit: Initial commit

↳ Output ↴
[master 1a2b3c4] Initial commit
 1 file changed, 1 insertion(+)
 create mode 100644 example.txt
```

# `NOTE : This is just a project to automate the basic steps that I generally do when pushing a project to a git repository`