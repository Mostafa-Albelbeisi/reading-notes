# Automation

A **regular expression** is a pattern that the regular expression engine attempts to match in input text. A pattern consists of one or more character literals, operators, or constructs.

## RegEx Functions:
- **findall**	Returns a list containing all matches
- **search**	Returns a Match object if there is a match anywhere in the string
- **split**	Returns a list where the string has been split at each match
- **sub**	Replaces one or many matches with a string

* In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import:
`import re`

## Shutil Module
### Copying Files to another directory
**shutil.copy()** method in Python is used to copy the content of the source file to the destination file or directory. It also preserves the file’s permission mode but other metadata of the file like the file’s creation and modification times is not preserved.

### Copying the Metadata along with File
**shutil.copy2()** method in Python is used to copy the content of the source file to the destination file or directory. This method is identical to shutil.copy() method but it also tries to preserve the file’s metadata.

### Copying the content of one file to another
**shutil.copyfile()** method in Python is used to copy the content of the source file to the destination file. The metadata of the file is not copied. Source and destination must represent a file and destination must be writable. If the destination already exists then it will be replaced with the source file otherwise a new file will be created.

### Copying the content of one file to another
**shutil.copyfile()** method in Python is used to copy the content of the source file to the destination file. The metadata of the file is not copied. Source and destination must represent a file and destination must be writable. If the destination already exists then it will be replaced with the source file otherwise a new file will be created.

### Removing a Directory
**shutil.rmtree()** is used to delete an entire directory tree, the path must point to a directory (but not a symbolic link to a directory).

### Finding files
**shutil.which()** method tells the path to an executable application that would be run if the given cmd was called. This method can be used to find a file on a computer which is present on the PATH.

## watchdog
**watchdog** is an open-source python API library that is a cross-platform API to monitor file system events. You can specify a folder or a directory to watchdog observer, which keeps monitoring the folder for any changes like file creation, modification, deletion, or moving of files from one folder to another.

* you can install watchdog as shown below:
`pip install watchdog`