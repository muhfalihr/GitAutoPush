# GitAutoPush

GitAutoPush is a simple bash script that allows you to easily add, commit, and push changes to your GitHub repository. With this script, you can perform basic git tasks quickly and efficiently, making your software development process smoother and more effective

## Program installation steps

1. Grant execution permission (execute)
    
    ```bash
    chmod +x gitautopush
    ```

2. Add the directory location of the gitautopush file to the `PATH` environment variable Create an environment variable for `GITHUB_ACCESS_TOKEN` in the files `~/.bashrc` ( **for bash shell** ), `~/.zshrc` ( **for zsh shell** ), `~/.config/fish/config.fish` ( **for fish shell** ). Because I use the ***zsh shell***, for this practice I edited the configuration in the `~/.zshrc` file.

    ```bash
    nano ~/.zshrc
    ```

    Add the **gitautopush directory** to the `PATH` environment variable

    ```bash
    export GITHUB_ACCESS_TOKEN=<github-access-token>
    export PATH=$PATH:/path/to/directory
    ```

    save changes to the `~/.zshrc` file

3. Set environment variables

    ```bash
    source ~/.zshrc
    ```

4. How to run this program

    ```bash
    gitautopush
    ```


# `NOTE : This is just a project to automate the basic steps that I generally do when pushing a project to a git repository`