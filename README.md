## Cleaner Script

### Description

Basically, we need to implement a file cleaner script that finds the latest version of a file with code in a folder, removes all the other files and adds them to .gitignore file. The script should take folder as an argument.

To find the format that developer is using to store his code we need to list all the unique formats in a folder, and select the most popular one.
From all files with that format we need to select a non-empty file, which has the biggest postfix in name(e.g., file8.ext from file1.ext...file8.ext) and latest modification date.
After the latest file with code has been found, all files other than the latest need to be removed from directory, and their extensions should be added in to .gitignore file.

In the end the script should print success message with the most popular format, successful .gitignore file creation, and amount of files that were removed.
