﻿[![Contributors][contributors-shield]][contributors-url][![Forks][forks-shield]][forks-url][![Stargazers][stars-shield]][stars-url][![Issues][issues-shield]][issues-url][![License][license-shield]][license-url][![LinkedIn][linkedin-shield]][linkedin-url]

# ![Logo][logo] Blazor For Beginners

A step-by-step guide to setting up a modern Blazor project using .NET 9.
This guide is ideal for developers new to Blazor or those looking for a clean project structure.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Project Setup Steps](#project-setup-steps)
  - [1. Create Folder Structure](#1-create-folder-structure)
  - [2. Create a New Solution](#2-create-a-new-solution)
  - [3. Create the Blazor Project](#3-create-the-blazor-project)
  - [4. Add Project to Solution](#4-add-project-to-solution)
- [Resulting Structure](#resulting-structure)
- [Next Steps](#next-steps)

## Introduction

This guide demonstrates how to create a scalable Blazor project using the terminal. Using the terminal provides more flexibility and control than Visual Studio or Visual Studio Code GUIs.

## Prerequisites

- [.NET 9 SDK](https://dotnet.microsoft.com/download/dotnet/9.0) installed
- Terminal access (Bash, PowerShell, or compatible)
- Visual Studio, Visual Studio Code or other C# ide

## Project Setup Steps

### Step 1 Create solution with an empty blazor project

#### 1. Create Folder Structure

Organize your solution and projects in a clean directory layout.
It's recommended to keep source files in a `src` subfolder.

```powershell
    mkdir Dotnet.BlazorForBeginners/src
    cd Dotnet.BlazorForBeginners
```

#### 2. Create a New Solution

Generate the solution file for your workspace:

```powershell
    dotnet new sln -n BlazorForBeginners
```

#### 3. Create the Blazor Project

Create an empty Blazor project targeting .NET 9 inside the `src` folder:

```powershell
    cd src
    dotnet new blazor --interactivity None --empty -n BlazorForBeginners.Frontend -f net9.0
```

- `--interactivity None`: Starts with a static server (no interactive features).
- `--empty`: Creates a minimal, empty project template.

#### 4. Add Project to Solution

Add the new Blazor project to your solution:

```powershell
    dotnet sln ../BlazorForBeginners.sln add BlazorForBeginners.Frontend/BlazorForBeginners.Frontend.csproj
```

#### Resulting Structure

After completing the steps, your directory should look like:

```powershell
BlazorForBeginners/
├── BlazorForBeginners.sln
    └── src/
        └── BlazorForBeginners.Frontend/
            └── BlazorForBeginners.Frontend.csproj
```

### Step 2

#### Next Steps

- Open the solution in Visual Studio or your preferred IDE.
- Start building your Blazor components in the `BlazorForBeginners.Frontend` project.
- Refer to the [official Blazor documentation](https://learn.microsoft.com/aspnet/

## Acknowledgments

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/Tirsvad/Dotnet.BlazorForBeginners?style=for-the-badge
[contributors-url]: https://github.com/Tirsvad/Dotnet.BlazorForBeginners/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Tirsvad/Dotnet.BlazorForBeginners?style=for-the-badge
[forks-url]: https://github.com/Tirsvad/Dotnet.BlazorForBeginners/network/members
[stars-shield]: https://img.shields.io/github/stars/Tirsvad/Dotnet.BlazorForBeginners?style=for-the-badge
[stars-url]: https://github.com/Tirsvad/Dotnet.BlazorForBeginners/stargazers
[issues-shield]: https://img.shields.io/github/issues/Tirsvad/Dotnet.BlazorForBeginners?style=for-the-badge
[issues-url]: https://github.com/Tirsvad/Dotnet.BlazorForBeginners/issues
[license-shield]: https://img.shields.io/github/license/Tirsvad/Dotnet.BlazorForBeginners?style=for-the-badge
[license-url]: https://github.com/Tirsvad/Dotnet.BlazorForBeginners/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/jens-tirsvad-nielsen-13b795b9/
[githubIssue-url]: https://github.com/Tirsvad/Dotnet.BlazorForBeginners/issues/
[repos-size-shield]: https://img.shields.io/github/repo-size/Tirsvad/Dotnet.BlazorForBeginners?style=for-the-badg

[logo]: https://raw.githubusercontent.com/Tirsvad/Dotnet.BlazorForBeginners/master/images/logo/32x32/logo.png