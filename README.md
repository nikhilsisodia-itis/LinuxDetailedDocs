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
      - The full path of a file or directory from the root directory. 
      - It used forward slash (/) as the separator. 
      - Use '/' after every directory name.
      - Example: `cd /home/username/Documents/file.txt`.
      - Absolute paths are more reliable.
    
    - Relative Paths:
      - The path of a file or directory relative to the current working directory.
      - It does not start with a forward slash (/).
      - Use '.' to represent the current directory.
      - Use '..' to represent the parent directory.
      - Example: `cd Documents/file.txt` (if the current directory is /home/username).
      - Relative paths are more convenient for navigating within the current directory.

## Module 3- Getting started with the Terminal:
- #### Opening the Terminal.
  - To open the terminal, you can use the following methods:
    + Press `Ctrl + Alt + T` on your keyboard.
    + Search for "Terminal" in your application menu or dashboard.
    + Right-click on the desktop or file manager and select "Open Terminal" or "Open in Terminal."
  - The terminal window will open, and you will see a command prompt where you can enter commands.

- #### Basic Terminal Shorcuts:
  + `ctrl + l`: Clear the terminal screen.
  + `ctrl + c`: Cancel the current command or process.
  + `ctrl + z`: Suspend the current command or process.
  + `ctrl + a`: Move the cursor to the beginning of the line.
  + `ctrl + e`: Move the cursor to the end of the line.
  + `ctrl + u`: Delete the line from the cursor to the beginning.
  + `ctrl + k`: Delete the line from the cursor to the end.
  + `ctrl + w`: Delete the word before the cursor.
  + `ctrl + r`: Search through command history.
  + `ctrl + d`: Log out of the current session or close the terminal.
  + `ctrl + shift + t`: Open a new terminal tab.
  + `ctrl + shift + n`: Open a new terminal window.
  + `ctrl + shift + c`: Copy selected text to the clipboard.
  + `ctrl + shift + v`: Paste text from the clipboard into the terminal.
  + `ctrl + shift + page up`: Scroll up in the terminal.
  + `ctrl + shift + page down`: Scroll down in the terminal.
  + `ctrl + shift + plus (+)`: Increase font size.
  + `ctrl + minus (-)`: Decrease font size.
  + `ctrl + 0`: Reset font size to default.
  + `ctrl + shift + q`: Close the terminal window.
  + `ctrl + left arrow`: Move the cursor one word to the left.
  + `ctrl + right arrow`: Move the cursor one word to the right.
  + `ctrl + shift + up arrow`: Scroll up one line.
  + `ctrl + shift + down arrow`: Scroll down one line.
  + `ctrl + shift + home`: Move the cursor to the beginning of the terminal buffer.
  + `ctrl + shift + end`: Move the cursor to the end of the terminal buffer.
  + `ctrl + shift + f`: Open the search bar to find text in the terminal.

- #### Basic Terminal Commands:
  - `pwd`: Print the current working directory.
  - `ls`: List files and directories in the current directory.
    - `ls <path_to_directory>`: List files and directories with detailed information.
  - `cd`: Change the current directory.
    - `cd <directory_name>`: Change to the specified directory.
    - `cd ..`: Move to the parent directory.
    - `cd ~`: Move to the home directory.
  - `mkdir`: Create a new directory.
    - `mkdir <directory_name>`: Create a new directory with the specified name.
  - `cp`: Copy files or directories.
    - `cp <source_file> <destination_file>`: Copy the source file to the destination file.
    - `cp -r <source_directory> <destination_directory>`: Copy the source directory and its contents to the destination directory.
  - `mv`: Move or rename files or directories.
    - `mv <source_file> <destination_file>`: Move the source file to the destination file.
  - `touch`: Create an empty file or update the timestamp of an existing file.
    - `touch <file_name>`: Create an empty file with the specified name.
  - `cat`: Concatenate and display the contents of a file.
    - `cat <file_name>`: Display the contents of the specified file.
  - `more`: View the contents of a file one screen at a time.
    - `more <file_name>`: View the contents of the specified file.
  - `less`: View the contents of a file with backward scrolling.
    - `less <file_name>`: View the contents of the specified file.
  - `head`: Display the first few lines of a file.
    - `head <file_name>`: Display the first 10 lines of the specified file.
  - `tail`: Display the last few lines of a file.
    - `tail <file_name>`: Display the last 10 lines of the specified file.
  - `echo`: Display a message or variable value in the terminal.
    - `echo $<variable_name>`: Display the specified message in the terminal.
  - `man`: Display the manual page for a command.
    - `man <command_name>`: Display the manual page for the specified command.
  - `clear`: Clear the terminal screen.
  - `history`: Display the command history.
  - `exit`: Exit the terminal or log out of the current session.
  - `whoami`: Display the current user's username.
  - `date`: Display the current date and time.
  - `uname`: Display system information, such as the kernel version and architecture.
  - `df`: Display disk space usage for file systems.
  - `du`: Display disk usage for files and directories.
  - `free`: Display memory usage information.
  - `top`: Display real-time system resource usage, including CPU and memory usage.
  - `ps`: Display information about running processes.
  - `kill`: Terminate a running process by its process ID (PID).
    - `kill <process_id>`: Terminate the specified process.
  
  ## Module 4- The 'ls' command in depth:
  - The `ls` command is used to list files and directories in the current directory or a specified directory.
    - `ls` stands for list.
  - `ls -l`: List files and directories with detailed information, including permissions, ownership, size, and modification date.
    - `-l` flag stands for long listing or long format.
  - `ls -a`: List all files and directories, including hidden files (those starting with a dot).
    - `-a` flag stands for all.
  - `ls -h`: Display file sizes in a human-readable format (e.g., KB, MB).
    - `-h` flag stands for human-readable.
  - `ls -R`: Recursively list files and directories in all subdirectories.
    - `-R` flag stands for recursive.
  - `ls -S`: Sort files and directories by size, with the largest first.
    - `-S` flag stands for size.
  - `ls -i`: Display the inode number of each file and directory.
    - `-i` flag stands for inode.
  - `ls -lt`: Sort files and directories by modification time, with the most recently modified first.
    - `-lt` flag stands for long format and time.
  - `ls -lu`: Sort files and directories by last access time, with the most recently accessed first.
    - `-lu` flag stands for last access time.
  - `ls -lc`: Sort files and directories by last status change time, with the most recently changed first.
    - `-lc` flag stands for last change time.
  - `ls -X`: Sort files and directories by extension.
    - `-X` flag stands for extension.
  - `ls -r`: Reverse the order of the listing.
    - `-r` flag stands for reverse. 
  - Original listing command without the alias:
    > `\ls`: Run the `ls` command without any aliases or functions that may have been defined in the shell.
  - Aliased `ls` command default colour coding:
    > Blue: Directory.
    > Green: Executable file.
    > Red: Archive file.
    > Cyan: Symbolic link.
    > Yellow: Device file.
    > Magenta: Image file.
    > White: Text file.

  ## Module 5- File types in Linux:
  - In Linux, files are categorized into different types based on their content and purpose. The main file types are:
    > .log files: Log files.
    > .txt files: Text files.
    > .conf files: Configuration files.
    > .sh files: Shell script files.
    > '-' denotes a regular file.
    > 'd' denotes a directory.
    > 'l' denotes a symbolic link.
    > 'c' denotes a character device file.
    > 'b' denotes a block device file.
    > 's' denotes a socket file.
    > 'p' denotes a named pipe file.
    > ls -F option: Display the file types.
    > '/' indicates a directory.
    > '@' indicates a symbolic link.
    > '|' indicates a named pipe file.
    > '*' indicates an executable file.
    > '=' indicates a socket file.
    > ' ' indicates a regular file.
  - To check the file type of a file, you can use the `file` command:
    > `file <file_name>`: Display the file type of the specified file.