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
---

## 📄 Input/Output and Text Processing

```bash
stdout (Standard Output)
echo "Hello" > file.txt      # Redirects output to a file (overwrites)

stdin (Standard Input)
cat                         # Takes input from keyboard until EOF (Ctrl+D)

stderr (Standard Error)
ls missing.txt 2> error.txt  # Redirects errors to a file

pipe and tee
ls -l | grep ".txt"         # Pipe output from one command into another
echo "test" | tee output.txt  # Write output to screen and file

env (Environment)
env                         # Show environment variables
printenv PATH               # Show specific variable

cut
cut -d',' -f1 file.csv      # Extract first field from CSV

paste
paste file1.txt file2.txt   # Combine lines from two files side by side

head
head -n 5 file.txt          # Show first 5 lines

tail
tail -n 5 file.txt          # Show last 5 lines

expand and unexpand
expand file.txt             # Convert tabs to spaces
unexpand file.txt           # Convert spaces to tabs

join and split
join file1.txt file2.txt    # Join lines with a common field
split -l 100 bigfile.txt    # Split file into 100-line chunks

sort
sort file.txt               # Sort lines alphabetically

tr (Translate)
tr 'a-z' 'A-Z' < file.txt   # Convert lowercase to uppercase

uniq (Unique)
uniq file.txt               # Remove adjacent duplicate lines

wc and nl
wc file.txt                 # Show word/line/character count
nl file.txt                 # Number each line

grep
grep "error" file.txt       # Search for lines containing 'error'

## 🚪 Exiting

```bash
exit   # Exit the terminal session
```
