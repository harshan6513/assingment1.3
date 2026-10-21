# Assignment 1.3: Terminal & Developer Workflow

## 1. Objective

The objective of this assignment is to learn how to create and manage folders and files using terminal commands and open a project in Visual Studio Code.

## 2. Introduction

A terminal is a text-based interface that allows users to interact with a computer by typing commands. Developers use the terminal to create folders, manage files, navigate between directories, and run development tools.

## 3. Procedure and Terminal Commands

The following commands are for Windows Command Prompt (CMD).

### Step 1: Open the Terminal

Open Command Prompt or the VS Code terminal.

### Step 2: Create the Project Folder

```bat
mkdir web-development-practice
cd web-development-practice
```

The `mkdir` command creates a folder, and `cd` changes the current directory.

### Step 3: Create Week Folders

```bat
mkdir week-1 week-2 week-3
```

This command creates three folders inside the project folder.

### Step 4: Create an index.html File in Each Folder

```bat
type nul > week-1\index.html
type nul > week-2\index.html
type nul > week-3\index.html
```

These commands create an empty `index.html` file inside each week folder.

### Step 5: Practice Navigation

```bat
cd week-1
cd ..
cd week-2
cd ..
```

The `cd` command navigates between folders, while `cd ..` moves one level up to the parent directory.

### Step 6: Practice Renaming a Folder

Return to the project folder if necessary, then run:

```bat
ren week-3 week-3-practice
ren week-3-practice week-3
```

The `ren` command renames a folder. The second command restores the original name.

### Step 7: Practice Deleting a Folder

**Caution:** Deleting a folder can permanently remove its contents. For safe practice, create and delete a separate empty test folder.

```bat
mkdir test-folder
rmdir test-folder
```

The `rmdir` command removes an empty directory.

### Step 8: Open the Project in VS Code

From inside the `web-development-practice` folder, run:

```bat
code .
```

This opens the current project folder in Visual Studio Code, provided the `code` command is available in the system PATH.

### Step 9: Verify the Final Folder Structure

Run:

```bat
tree /F
```

This command displays the folder structure, including files.

## 4. Expected Folder Structure

```text
web-development-practice
│
├── week-1
│   └── index.html
│
├── week-2
│   └── index.html
│
└── week-3
    └── index.html
```

## 5. Result

I learned how to create folders and files, navigate between directories, rename folders, delete an empty test folder, and open a project in Visual Studio Code using terminal commands. I also learned how to verify the final project structure using the `tree /F` command.