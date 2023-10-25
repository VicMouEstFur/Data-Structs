# Data-Structs

This repository contains a Go project and is set up with GitHub Actions for automated build and test workflows. Additionally, when working on this project in VS Code, there are custom tasks and keybindings set up for streamlined Git operations.

## Project Structure

- **Go code files**: All Go-related source files.
- **`.github/workflows/run_go_code.yml`**: GitHub Actions workflow to run the Go code on every push to the `main` branch.
- **`.vscode/tasks.json`**: Defines custom tasks in VS Code, specifically the `pushToMain` task for Git operations.
- **`.vscode/keybindings.json`**: Specifies custom keybindings in VS Code, particularly the shortcut to run the `pushToMain` task.

## GitHub Actions Workflow

The GitHub Actions workflow is designed to:

1. Set up a Go environment.
2. Install any project dependencies.
3. Run the `main.go` file.

This workflow is triggered on every `push` and `pull_request` to the `main` branch.

## Custom Tasks in VS Code

There's a custom task named `pushToMain` which automates the process of adding changes to Git, committing with a specific message, and pushing to the `main` branch. This task is defined in the `.vscode/tasks.json` file.

To run the task:

- Use the command palette (`Ctrl + Shift + P`), type "Tasks: Run Task", and select the `pushToMain` task.
- Or, use the custom keybinding `Ctrl + Alt + P`.

## Custom Keybindings in VS Code

A custom keybinding is set up for the `pushToMain` task, allowing you to quickly run the task with a keyboard shortcut. This keybinding is defined in the `.vscode/keybindings.json` file.

**Shortcut**: `Ctrl + Alt + P`

This shortcut is project-specific and will only be active when you have the `Data-Structs` project opened in VS Code.

## Getting Started with PowerShell

1. **Open PowerShell**:
   
   Press `Windows + X` and select `Windows PowerShell`.

2. **Navigate to Your Preferred Directory**:

   Use the `Set-Location` command to navigate to the directory where you want to clone the repository:
   ```powershell
   Set-Location -Path "C:\path_to_your_preferred_directory"