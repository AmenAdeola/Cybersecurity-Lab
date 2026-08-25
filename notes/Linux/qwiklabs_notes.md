# Qwiklabs Notes

## Lab: Linux Shell Basics

### Objective

Learn basic Bash shell commands used to generate output, perform calculations, and manage the terminal display.

------------

# commands Learned

## echo

Purpose
Display text in the shell.

Example:
''' bash
echo hello 
'''

Output:
'''text
hello
'''

Example with quotation marks:

'''bash 
echo "hello"
'''

Output:
'''text
hello
'''

Notes:
Quotation marks group text together and are useful when strings contain spaces or special characters.

---------

## expr

Purpose:
Perform simple mathematical calculation from the command line

Example:
'''bash
expr 32 - 8
'''

Ouput:

'''text
24
'''

Notes:
The expr command requires spaces between numbers and operators.

Correct;

'''bash
expr 32 - 8
'''

Incorrect syntax:

''' bash
expr 32-8

Use cases:
-  Calculate alert statistics
-  Quick arithmetic from the shell
-  Security metrics calculations

-----------

## clear

Purpose ;
clear the terminal screen.

Exmaple:

'''bash
clear
'''

Result;
All previous output is removed from the visible terminal window and the cursor returns to the top.

Use cases:
-  Reduce clutter
-  Improve readability
-  Start a new task with a clean screen

----------------
# Concept learned

## Shell

A shell is command-line interpretor that allows users to interact with the operating system.

Examples:

-  Bash
-  Zsh
-  Sh
-  PowerShell

---------------
## Terminal

A terminal is the application window that provides access to a shell.

Key Difference:

Terminal = Window

Shell = Command Interpreter

-------------

# Key Takeways

-  echo displays text output.
-  expr performs simple calculations.
-  clear removes terminal output from view.
-   Bash is a command-line shell by default
-   The terminal provides access to the shell.
Qu
