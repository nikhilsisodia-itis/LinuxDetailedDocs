# Detailed Documentation of Linux.

This is a detailed documentation of Linux commands, including their usage, options, and examples. It is designed to be a comprehensive resource for users of all levels, from beginners to advanced users.

## Module 1- Introduction to Linux:

- #### What is Linux?
  - Linux is a family of open-source Unix-like operating systems based on the Linux kernel. It is widely used for servers, desktops, and embedded systems.
  - Linux is known for its stability, security, and flexibility. It is used by millions of users around the world and has a large community of developers and users who contribute to its development and support.

- #### Why use Linux?
  - Linux is free and open-source, which means that anyone can use, modify, and distribute it.
  - It is highly customizable, allowing users to tailor their operating system to their specific needs.
  - Linux is known for its security and stability, making it a popular choice for servers and critical systems.
  - It has a large community of users and developers who provide support and contribute to its development.

- #### Linux VS Unix.
  - Linux is a Unix-like operating system, meaning it shares many similarities with Unix but is not derived from the original Unix code.
  - Linux is open-source and free to use, while Unix is a proprietary operating system that requires a license.
  - Linux has a large community of developers and users, while Unix is typically used in enterprise environments with commercial support.

- #### What is Open Source?
  - Open source refers to software that is released with a license that allows users to view, modify, and distribute the source code.
  - Open source software is often developed collaboratively by a community of developers and users, which leads to rapid development and innovation.
  - Examples of open source software include the Linux kernel, the Apache web server, and the Mozilla Firefox web browser.

  - #### What is Source Code?
    - Source code is the human-readable version of a computer program. It is written in a programming language and can be compiled or interpreted to create an executable program.
    - Source code is often distributed with open source software, allowing users to view and modify the code.
    - Examples of programming languages include C, C++, Python, and Java.

- #### What is a Kernel?
  - The kernel is the core component of an operating system. It manages the system's resources and provides a bridge between the hardware and software.
  - The Linux kernel is the heart of the Linux operating system. It is responsible for managing hardware resources, such as memory, CPU, and I/O devices.
  - The kernel also provides a set of system calls that allow user programs to interact with the hardware and perform tasks such as file I/O, process management, and network communication.

- #### What is a Shell?
  - A shell is a command-line interface that allows users to interact with the operating system. It provides a way to execute commands, run programs, and manage files.
  - The shell interprets user commands and translates them into actions that the operating system can perform.
  - There are many different shells available for Linux, including Bash, Zsh, and Fish. Each shell has its own features and syntax, but they all provide similar functionality.

- #### What is a Command Line Interface (CLI)?
  - A command line interface (CLI) is a text-based interface that allows users to interact with the operating system by typing commands.
  - The CLI is often used for system administration tasks, scripting, and automation.
  - The CLI is powerful and flexible, allowing users to perform complex tasks with simple commands. However, it can be intimidating for new users who are more familiar with graphical user interfaces (GUIs).

- #### What is a Graphical User Interface (GUI)?
  - A graphical user interface (GUI) is a visual interface that allows users to interact with the operating system using graphical elements such as windows, icons, and menus.
  - GUIs are often more user-friendly than command line interfaces, making them easier for new users to navigate.
  - However, GUIs can be less efficient for advanced users who prefer the speed and flexibility of the command line.

- #### What is a Terminal?
  - A terminal is a text-based interface that allows users to interact with the operating system using a command line interface.
  - Terminals are often used to run shell commands, execute scripts, and manage files.
  - Terminals can be accessed through a graphical user interface or through a remote connection using SSH (Secure Shell).

- #### Terminal, Console, Shell, & Commands.
  - A terminal is a text-based interface that allows users to interact with the operating system using a command line interface.
  - A console is a physical or virtual terminal that provides access to the operating system.
  - A shell is a program that interprets user commands and translates them into actions that the operating system can perform.
  - Commands are instructions that users type into the shell to perform specific tasks, such as creating files, managing processes, and configuring the system.

- #### Parts of a Command.
  - A command typically consists of three parts: the command name, options (or flags), and arguments.
  - The command name is the name of the program or utility that you want to run.
  - Options (or flags) are optional parameters that modify the behavior of the command. They usually start with a hyphen (-) or double hyphen (--).
  - Arguments are the input or target for the command, such as file names or directories.
  - Example: `ls -l /home/user` where `ls` is the command name, `-l` is an option, and `/home/user` is an argument.

## Module 2- The Linux File System:

- #### What is a File System?
  - A file system is a method of organizing and storing files on a storage device, such as a hard drive or SSD.
  - The file system defines how files are named, stored, and accessed, as well as how directories are structured.
  - Linux supports several file systems and each file system has its own features and performance characteristics, making it suitable for different use cases.

- #### Linux File System Hierarchy.
  - The Linux file system hierarchy is organized in a tree-like structure, with the root directory (/) at the top and various subdirectories below it.
  - Common directories include:
    + `/bin`: Contains essential command-line utilities and programs.
    + `/sbin`: Contains system administration commands and utilities.
    + `/boot`: Contains files needed to boot the system, including the kernel and bootloader.
    + `/home`: Contains user home directories, where users store their personal files and settings.
    + `/dev`: Contains device files that represent hardware devices on the system.
    + `/etc`: Contains system configuration files and settings.
    + `/lib`: Contains shared libraries and kernel modules needed by programs.
    + `/media`: Contains mount points for removable media, such as USB drives and CD-ROMs.
    + `/mnt`: Contains mount points for temporarily mounted file systems.
    + `/opt`: Contains optional software packages and applications.
    + `/proc`: Contains virtual files that provide information about system processes and kernel parameters.
    + `/root`: The home directory for the root user (system administrator).
    + `/run`: Contains runtime data and information about the system's current state.
    + `/srv`: Contains data for services provided by the system, such as web servers and databases.
    + `/tmp`: Contains temporary files created by programs and users.
    + `/usr`: Contains user-related programs and data, including applications and libraries.
    + `/var`: Contains variable data, such as log files, mail spools, and temporary files.
  - The file system hierarchy is designed to be consistent and predictable, making it easier for users and administrators to navigate and manage files.
    
  - Absoulte VS Relative Paths:
    - Absolute Paths:
      The full path of a file or directory from the root directory. 
      It used forward slash (/) as the separator. 
      Use '/' after every directory name.
      Example: `cd /home/username/Documents/file.txt`.
      Absolute paths are more reliable.
    
    - Relative Paths:
      The path of a file or directory relative to the current working directory.
      It does not start with a forward slash (/).
      Use '.' to represent the current directory.
      Use '..' to represent the parent directory.
      Example: `cd Documents/file.txt` (if the current directory is /home/username).
      Relative paths are more convenient for navigating within the current directory.