# Check Ignore

`git check-ignore` is a useful command when using the `.gitignore` feature.

## Example Use

![img](example-chk-ig.png)

_Image of `check-ignore` being used_

## Background Information

`.gitignore` is a file that identifies the files or folders that you do not want tracked by git. This will exclude the files and folders from showing up in the working directory or staging area and will not be pushed to remote repositories.

## Use Case

When working on a project with a `.gitignore` file, it might be needed to identify why a file is not being displayed in the working directory or staging area while working on a project. The `git check-ignore` command will allow you to quickly identify if specific files or folders are included in the `gitignore` file.

## Helpful Options

`-v`: displays more information about how the `.gitignore` file reference the file or folder in question.
