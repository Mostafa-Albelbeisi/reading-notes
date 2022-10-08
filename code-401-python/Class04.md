# Reading and Writing Files in Python
**File:**
file could be a contiguous set of bytes wont to store knowledge, these computer memory unit files ar then translated into binary one and zero for easier process by the pc, and may be something as straightforward as a document or as difficult as a program practicable.

file systems are composed of three main parts:
- Header: metadata about the contents of the file (file name, size, type, and so on)
- Data: contents of the file as written by the creator or editor
- End of file (EOF): special character that indicates the end of the file

**The file path is a string that represents the location of a file, a file path is required. It’s broken up into three major parts:**
- Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix).
- File Name: the actual name of the file
- Extension: the end of the file path pre-pended with a period (.) used to indicate the file type

# Opening and Closing a File in Python
It’s important to remember that it’s your responsibility to close the file. In most cases, upon termination of an application or script, a file will be closed eventually. However, there is no guarantee when exactly that will happen. This can lead to unwanted behavior including resource leaks. It’s also a best practice within Python (Pythonic) to make sure that your code behaves in a way that is well defined and reduces any unwanted behavior.

# Python Exceptions
- A **syntax error** occurs when a programmer writes an incorrect line of code. Most syntax errors involve missing punctuation or a misspelled name. If there is a syntax error in a compiled or interpreted programming language, then the code won't work.

- **Assertion error** is a programming concept used while writing a code where the user declares a condition to be true using assert statement prior to running the module. If the condition is True, the control simply moves to the next line of code. In case if it is False the program stops running and returns AssertionError Exception.

![ad](Screenshot%202022-10-08%20172731.png)