# Unity - Format - Checker

## Description

The **Unity - Format - Checker** is a GitHub Action that automatically checks the format of your Unity project's C# code. It generates a temporary project file, validates the code using .NET formatting tools, and cleans up the temporary files after the check.

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