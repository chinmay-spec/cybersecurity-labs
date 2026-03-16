# Linux Basics Lab – Day 1

## Objective

Learn basic Linux commands used in ethical hacking environments and understand how to navigate the Linux terminal.

## Lab Environment

Operating System: Parrot OS
Virtualization: UTM on MacBook M1

## Commands Practiced

whoami
hostname
pwd
ls
ls -l
cd
cd ..
cd ~
clear
history

## Command Explanation

**whoami**
Displays the username of the currently logged-in user.

**hostname**
Shows the system's hostname (the name of the machine on a network).

**pwd (Print Working Directory)**
Displays the full path of the current directory you are working in.

Example:
pwd

Output:

```
/home/chinmay
```

**ls (List Files)**
Lists all files and directories in the current directory.

Example:
ls

**ls -l (Long Listing Format)**
Displays detailed file information including:

* File permissions
* Owner
* File size
* Last modified date

Example:
ls -l

**cd (Change Directory)**
Used to move between directories.

Example:
cd Documents

**cd ..**
Moves one level up in the directory structure.

Example:
cd ..

**cd ~**
Returns to the user's home directory.

Example:
cd ~

**clear**
Clears the terminal screen to make the interface easier to read.

Example:
clear

**history**
Displays a list of previously executed commands in the terminal.

Example:
history

## Key Takeaways

Learning Linux command-line navigation is essential for cybersecurity professionals. Most penetration testing and security tools operate through the terminal, and understanding these commands allows efficient interaction with the system.

These commands are frequently used while performing:

* System navigation
* File analysis
* Running security tools
* Managing penetration testing environments

## Next Steps

Continue strengthening Linux fundamentals by learning:

* File creation and editing
* File permissions
* User management
* Networking commands

Future labs will focus on networking concepts and security tools used in penetration testing.
