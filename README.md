# Unity Format Checker

## Description

The **Unity Format Checker** is a GitHub Action that automatically checks the format of your Unity project's C# code. It generates a temporary project file, validates the code using .NET formatting tools, and cleans up the temporary files after the check.

## Features

- Checks the format of C# scripts in your Unity project.
- Supports customization of the target directory for script files.
- Automatically generates and deletes temporary project files.

## Inputs

| Input              | Description                                              | Default             |
|--------------------|----------------------------------------------------------|---------------------|
| `target_directory` | The directory containing the C# scripts to check.       | `Assets/Scripts`    |

## Outputs

| Output    | Description                                       |
|-----------|---------------------------------------------------|
| `formatted` | Indicates whether the formatting check was successful or not. |

## Usage

To use this action in your GitHub repository, create or update your workflow file (e.g., `.github/workflows/format-check.yml`) with the following content:

### Create an .editorconfig File

First, ensure you have a `.editorconfig` file at the root of your project to define your coding style preferences:
https://github.com/sangwookyoo/unity-format-checker/blob/master/.editorconfig

### Create a .gitattributes File

Next, add a `.gitattributes` file at the root of your project to manage line endings properly across different operating systems:
https://github.com/sangwookyoo/unity-format-checker/blob/master/.gitattributes
