# Linux CLI Practice

A collection of useful Linux commands I practiced while learning.

## 📁 File and Directory Navigation

```bash
ls -al       # List all files (including hidden ones) in long format
pwd          # Print current working directory
cd           # Change to a different directory
mkdir -p     # Create new directories, including parent directories
rmdir        # Remove a directory
```

## 📄 File Creation and Manipulation

```bash
touch file.txt          # Create a new file or update its timestamp
cp file.txt /path/      # Copy a file to another directory
mv file.txt newname.txt # Rename or move a file
rm file.txt             # Delete a file
```
## 🔍 Viewing and Identifying Files

```bash
file file.txt     # Determine file type
cat file.txt      # Print file contents
less file.txt     # View large file content page-by-page
```

## 🔎 Searching and Information

```bash
find ~ -name "*.txt"      # Find all .txt files in the home directory
find . -type d            # Find all directories in current path
history                   # Show command history
clear                     # Clear the terminal screen
```

## 📘 Help and Documentation

```bash
help cd          # Show help for built-in commands
ls --help        # Show options for external command
man ls           # Open the manual for a command
whatis ls        # Get a short description of a command
```

## ⚙️ Custom Commands (Aliases)

```bash
alias ll='ls -la'         # Create a shortcut command
unalias ll                # Remove an existing alias
```
## 🚪 Exiting

```bash
exit   # Exit the terminal session
```
