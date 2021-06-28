# Using Python to Interact with the Operating System
This course will teach how to use Python to perform system administration tasks and interact with a computer’s operating system. For some exercises the application called Qwiklabs is going to be used in a remote Linux virtual machine.

# Week 1 - Getting Your Python On
## Learning Objectives:
- Have an understanding of the different operating systems
- Utilize their Python environment and install additional Python modules, if needed
- Run Python locally on their machines
- Understand the benefits of automation but be aware of the pitfalls
- Complete all assessments through Qwiklabs

## Course prerequisites
- The basic Python syntax (if, for, while, defining functions, classes, and methods)
- How to use the most common data structures (strings, lists, tuples, and dictionaries)
- How to import and use additional Python modules

This course also requires some familiarity with some basic operating system concepts:
- Files, directories, and file systems
- Processes
- Log files

### Downloads and Imports
Windows:
- Python 3
- pip install requests> python> import requests 

More informations: https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/  
Installation guide for other OS: https://realpython.com/installing-python/

### Commands
python -V  
python --version

### Programming resources to study
- Automate the Boring Stuff with Python: This book (available online and in print) includes a lot of practical programming exercises for beginners. You can refer to this content to read more about some of the things that we'll be discussing, and get inspired with more ideas of things that can be automated.

- Hitchhiker’s Guide to Python: This site (available online and in print) also covers a lot of what we can do with Python. Again, you can use this resource to learn more about the subjects we cover (and the ones we had to omit for time constraints).

- The official language reference: Once you know what Python tool you'll be using to do a certain task, this technical reference of all Python language components can be a great   

## Getting Ready for Python
Operating System: The software that manages everything that goes on in the computer. It reads, writes and deletes files from the hard drive.

There are two main parts in an OS: the kernel and the user space.

**- Kernel:** 
The main core of an operating system. It talks directly to our hardware and manages our systems resources. As users, we don't interact with the kernel directly. Instead, we interact with the other part of the operating system called the user space. 
**- The User space:**
It is basically everything outside of the kernel. These are things that we interact with directly, like the system programs and user interface. 

When we say "operating system", we're referring to both the kernel and the user space. 

### Operating Systems
- Windows 
- MacOS
- Android
- FreeBSD
- Linux
    Distributions:
    - Ubuntu
    - Debian
    - Red Hat

### Python Modules
Python Modules are written and posted on  Python Package Index (PyPI) by programmers.
- pip: a command line tool used to install, update, and remove external modules on whichever operating system you're running on your computer. It's considered the main Python package manager. 

## Running Python Locally
### Interpreted Language x Compiled Language
### Interpreted Language
Programs written in interpreted language generally **rely on an intermediary program called an interpreter**. These programs use interpreters to execute the instructions specified in the code. 
- A compiler is not needed in this process, what makes the development cycle for a program written in an interpreted language much faster
- The code can be read by interpreters running on different operating systems without needing to make any additional changes. 
- Interpreted languages **generally run slower than compiled ones***  
*Examples: Python, Ruby, JavaScript, Bash and PowerShell*
 
### Compiled Language
- The source code is fed into a a compiler
- The compiler translates the code into  a specific machine level language, **depending on the computer OS**   
- After compiling, the computer can read and execute the machine level code directly  
- The compiled program is **super fast to run**, but **the compilation process itself can take a bit of time** 
*Examples of compiled programming languages: C, C++, Go and Rust*

* Java and C# are languages that use a mixed approach.  
### How to Run a Python Script
### Linux Commands - nano editor
*shebang*: specifies to the OS what command to use when running the script - in this case, we want to run the script using Python 3
*cat*: shows the contents of a file on Linux (e.g. 'cat areas.py')
*!/usr/bin/env python3*: tells the OS that we want to run the script using Python 3

### Code Reuse
e.g.:
python 3> import areas> areas.triangle(3,5)  
ls -l /usr/lib/python3/dist-packages/requests
__init__.py

### IDE - Integrated Development Environment
- *Syntax highlighting*: the language we are writing our code in, and highlights the pieces of code that make up the syntax of the language
- *Code completion*: automatically complete the names of the variables, functions and indentation spaces
- *Doughnut*: calculate the area of a 2-D doughnut as the difference between two circles   

## Automating Tasks Through Prgramming
- *Scalability*: when more work is added to a system, the system can do whatever it need to get the work done

### Pitfalls of Automation
#### "Is the time and the effort needed to write the script worth the potential automation benefits?"
- *Pareto Principle*: states 20% of the tasks that represents 80% of the work
- *Bit-rot*: the process of software falling out of step with the environment
- *Avoiding silent fallures*: by building a method or notification into the automated systems
- *Periodic tests*: needed to check in the behaviour of the automated systems to prevent further data corruption
- *Forensic value*: it is important for automated processes to leave extensive logs so when errors occur they can be an extremely useful source of information when you are investigating an issue

*Is is worth the time?* Check: https://xkcd.com/1205/

### QWiklabs
SSH: command that allows you to interact with remote Linux computers


