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
echo "Hello" > file.txt        # Redirects standard output to a file (overwrites)
cat                            # Takes standard input from keyboard until EOF (Ctrl+D)
ls missing.txt 2> error.txt    # Redirects standard error to a file
ls -l | grep ".txt"            # Pipes output from one command into another
echo "test" | tee output.txt   # Outputs to both terminal and file
env                            # Displays all environment variables
printenv PATH                  # Displays the value of a specific environment variable
cut -d',' -f1 file.csv         # Extracts the first field from a CSV file
paste file1.txt file2.txt      # Combines lines from two files side by side
head -n 5 file.txt             # Displays the first 5 lines of a file
tail -n 5 file.txt             # Displays the last 5 lines of a file
expand file.txt                # Converts tabs to spaces
unexpand file.txt              # Converts spaces to tabs
join file1.txt file2.txt       # Joins lines of two files on a common field
split -l 100 bigfile.txt       # Splits a file into chunks of 100 lines each
sort file.txt                  # Sorts lines in a file alphabetically
tr 'a-z' 'A-Z' < file.txt      # Translates lowercase to uppercase characters
uniq file.txt                  # Removes adjacent duplicate lines
wc file.txt                    # Displays word, line, and character count
nl file.txt                    # Adds line numbers to each line of a file
grep "error" file.txt          # Searches for lines containing the word 'error'
```
## 📄 Advanced Text Processing (Vim)

```bash
vim                 # Opens the vim editor 
vim fileName        # Opens a file with the vim editor 

vim commands:
/text               # Searches the text file for the keyword

i - insert text before the cursor
O - insert text on the previous line
o - insert text on the next line
a - append text after the cursor
A - append text at the end of the line

x - used to cut the selected text also used for deleting characters
dd - used to delete the current line
y - yank or copy whatever is selected
yy - yank or copy the current line
p - paste the copied text before the cursor

:w - writes or saves the file
:q - quit out of vim
:wq - write and then quit
:q! - quit out of vim without saving the file
ZZ - equivalent of :wq, but one character faster


```



## 🚪 Exiting

```bash
exit   # Exit the terminal session
```
