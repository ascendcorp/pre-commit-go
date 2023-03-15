# Pre-commit Hooks for ACW Project

This repository contains pre-commit hooks for Golang projects.

## How to Use

To use these pre-commit hooks in your Golang project, follow these steps:

1. Install the `pre-commit` tool by running `pip install pre-commit` in your terminal.
2. Create a `.pre-commit-config.yaml` file in the root of your project with the following contents:

   ```yaml
   repos:
     - repo: https://bitbucket.org/<YOUR_USERNAME>/<YOUR_REPOSITORY_NAME>
       rev: <COMMIT_HASH>  # Replace with the commit hash of the latest version of this repository
       hooks:
         - id: go-sec
         - id: dependency-check
3. Run `pre-commit install` in your terminal to install the pre-commit hooks in your local repository.
4. Commit the `.pre-commit-config.yaml` file to your repository.
5. Now, every time you run `git commit`, the pre-commit hooks will automatically run and check your code for security vulnerabilities and outdated dependencies.

## How to Contribute

To contribute to this repository, follow these steps:

1. Fork this repository on Bitbucket.
2. Clone your forked repository to your local machine.
3. Create a new branch for your changes: `git checkout -b my-new-branch`.
4. Make your changes and commit them: `git commit -am 'Add some feature'`.
5. Push your changes to your forked repository: `git push origin my-new-branch`.
6. Create a pull request from your forked repository to this repository.
7. Wait for the maintainers to review and merge your pull request.
