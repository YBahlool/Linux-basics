# Linux CLI Practice

A collection of useful Linux commands I practiced while learning.

## 🔧 Basic Commands
```bash
ls -al    # List all files (including hidden files) in the directory
pwd       # Prints the current directory you are working in
cd        # If followed by a directory inside of your working one, goes there
touch     # If followed by a file name will create that file in your current directory or update an existing files timestamps
file      # If followed by an existing file name, will return the files type
cat       # If followed by an existing files name, will return text written inside of it
less      # USed for reading through larger text files
history   # Returns every command that you have previously entered
clear     # clears the current terminal
cp        # If followed by an existing files name and then a directory will copy said file to the directory
mv        # Can be used to rename a file or directory or move a file to a different directory
mkdir     # Can be used to make new directories or sub directories using -p
rm        # Removes a file
rmdir     # Removes a directory
find      # Used to find a file must be followed by home directory and -name if searching by name or -type if searching by type
help      # Used to give information about bash commands, for commands like ls follow them by --help for info
man       # When followed by a command gives a manual for how the command works
whatis    # When followed by a command gives a small description of the command
alias     # When followed by a name and an equal sign (random='ls -la') it will allow you to use that name as that command
unalias   # When followed by an existing alias will remove the alias
exit      # Used to quit the terminal
