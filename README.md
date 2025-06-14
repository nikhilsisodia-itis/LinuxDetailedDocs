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

  ## Module 6- The 'cd' command in depth:

  - The `cd` command is used to change the current working directory in the terminal.
    - `cd` stands for change directory.
  - `cd <directory_path>`: Change to the specified directory.
    - The path can be absolute or relative.
  - `cd ..`: Move to the parent directory.
  - `cd ~`: Move to the home directory.
  - `cd -`: Change to the previous directory.
  - `cd /`: Change to the root directory.

  ## Module 7- Viewing files:

  ### 1. The `cat` command:
    - The `cat` command is used to concatenate and display the contents of a file.
    - `cat <file_name>`: Display the contents of the specified file.
    - The `cat` command is used to concatenate and display the contents of a file.
    - `cat <file_name>`: Display the contents of the specified file.
    - `cat -n <file_name>`: Display the contents of the file with line numbers.
    - `cat <file1> <file2>`: Concatenate and display the contents of multiple files.
    - `cat <file_name> > <output_file>`: Redirect the contents of the file to a new file.
    - `cat <file_name> >> <output_file>`: Append the contents of the file to an existing file.
    - `cat <file_name> | <command>`: Pipe the contents of the file to another command for further processing.

  ### 2. The `less` command:
    - less command: Display the contents of a file page by page.
    - less -N option: Display the line numbers.
    - less -X option: Do not clear the screen on exit.
    - less -S option: Truncate long lines.
    - ctrl + f: Move forward one page.
    - ctrl + b: Move backward one page.
    - g or <: Move to the beginning of the file.
    - G or >: Move to the end of the file.
    - / <pattern>: Search for a pattern.
    - n: Move to the next occurrence of the pattern.
    - N: Move to the previous occurrence of the pattern.
    - q: Quit the less command.
    - ? <pattern>: Search backward for a pattern.
  
  ### 3. The `more` command:
  - The `more` command is used to view the contents of a file one screen at a time.
  - `more <file_name>`: Display the contents of the specified file.
  - `more -d <file_name>`: Display a message when the end of the file is reached.
  - `more -c <file_name>`: Clear the screen before displaying the file.
  - `more -n <number_of_lines> <file_name>`: Display the specified number of lines at a time.

  ### 4. The `head` command:
  - The `head` command is used to display the first few lines of a file.
  - `head <file_name>`: Display the first 10 lines of the specified file.
  - `head -n <number_of_lines> <file_name>`: Display the specified number of lines from the beginning of the file.

  ### 5. The `tail` command:
  - The `tail` command is used to display the last few lines of a file.
  - `tail <file_name>`: Display the last 10 lines of the specified file.
  - `tail -n <number_of_lines> <file_name>`: Display the specified number of lines from the end of the file.
  - `tail -f <file_name>`: Continuously monitor the file for new lines as they are added (useful for log files).
  - `tail -c <number_of_bytes> <file_name>`: Display the specified number of bytes from the end of the file.
  - `tail -q <file1> <file2>`: Display the contents of multiple files without repeating the file names.
  - `tail -v <file1> <file2>`: Display the contents of multiple files with the file names.
  - `tail -r <file_name>`: Display the contents of the file in reverse order.
  - `tail -s <number_of_lines> <file_name>`: Display the specified number of lines from the end of the file, skipping empty lines.

  ## Module 8- Creating directories and files:

  ### 1. The `mkdir` command:
  - The `mkdir` command is used to create new directories.
  - `mkdir <directory_name>`: Create a new directory with the specified name.
  - `mkdir -p <directory_path>`: Create a directory and any necessary parent directories.
  - `mkdir -v <directory_name>`: Display a message when the directory is created.
  - `mkdir -m <permissions> <directory_name>`: Create a directory with the specified permissions.
  - `mkdir -i <directory_name>`: Prompt before creating a directory if it already exists.

  ### 2. The `touch` command:
  - The `touch` command is used to create empty files or update the timestamp of existing files.
  - `touch <file_name>`: Create an empty file with the specified name.
  - `touch -a <file_name>`: Update the access time of the file.
  - `touch -m <file_name>`: Update the modification time of the file.
  - `touch -c <file_name>`: Do not create a new file if it does not exist.
  - `touch -r <reference_file> <file_name>`: Set the timestamp of the file to match the reference file.
  - `touch -d <date_time> <file_name>`: Set the timestamp of the file to the specified date and time.
  - `touch -t <timestamp> <file_name>`: Set the timestamp of the file to the specified timestamp.

  ## Module 9- Copying and moving files:

  ### 1. The `cp` command:
  - The `cp` command is used to copy files and directories.
  - `cp <source_file> <destination_file>`: Copy the source file to the destination file.
  - `cp -r <source_directory> <destination_directory>`: Copy the source directory and its contents to the destination directory.
    - The `-r` flag stands for recursive, which means it will copy all files and subdirectories within the source directory.
  - `cp -i <source_file> <destination_file>`: Prompt before overwriting an existing file.
    - `-i` flag stands for interactive.
  - `cp -u <source_file> <destination_file>`: Copy the source file only if it is newer than the destination file.
    - `-u` flag stands for update.
  - `cp -v <source_file> <destination_file>`: Display a message when the file is copied.
    - `-v` flag stands for verbose.
  - `cp -a <source_file> <destination_file>`: Copy the file and preserve its attributes (permissions, timestamps, etc.).
    - `-a` flag stands for archive.
  - `cp -l <source_file> <destination_file>`: Create a hard link to the source file instead of copying it.
    - `-l` flag stands for link.
  - `cp -s <source_file> <destination_file>`: Create a symbolic link to the source file instead of copying it.
    - `-s` flag stands for symbolic link.
  - `cp -n <source_file> <destination_file>`: Do not overwrite an existing file.
    - `-n` flag stands for no clobber.
  - `cp -p <source_file> <destination_file>`: Preserve the file attributes (permissions, timestamps, etc.) when copying.
    - `-p` flag stands for preserve.
  - `cp -x <source_directory> <destination_directory>`: Copy only files from the same file system.
    - `-x` flag stands for one file system.

  ### 2. The `mv` command:
  - The `mv` command is used to move or rename files and directories.
  - `mv <source_file> <destination_file>`: Move the source file to the destination file.
  - `mv <source_file> <destination_directory>`: Move the source file to the specified directory.
  - `mv <source_directory> <destination_directory>`: Move the source directory and its contents to the destination directory.
  - `mv -i <source_file> <destination_file>`: Prompt before overwriting an existing file.
    - `-i` flag stands for interactive.
  - `mv -u <source_file> <destination_file>`: Move the source file only if it is newer than the destination file.
    - `-u` flag stands for update.
  - `mv -v <source_file> <destination_file>`: Display a message when the file is moved.
    - `-v` flag stands for verbose.
  - `mv -n <source_file> <destination_file>`: Do not overwrite an existing file.
    - `-n` flag stands for no clobber.
  - `mv -p <source_file> <destination_file>`: Preserve the file attributes (permissions, timestamps, etc.) when moving.
  - `mv -f <source_file> <destination_file>`: Force the move operation without prompting.
    - `-f` flag stands for force.
  - `mv -b <source_file> <destination_file>`: Create a backup of the destination file before overwriting it.
    - `-b` flag stands for backup.

  ## Module 10- Removing files and directories:
  
  ### 1. The `rm` command:
  - The `rm` command is used to delete files and directories.
  - `rm <file_name>`: Delete the specified file.
  - `rm -i <file_name>`: Prompt before deleting the file.
    - `-i` flag stands for interactive.
  - `rm -f <file_name>`: Force the deletion of the file without prompting.
    - `-f` flag stands for force.
  - `rm -r <directory_name>`: Recursively delete the specified directory and its contents.
    - `-r` flag stands for recursive.
  - `rm -v <file_name>`: Display a message when the file is deleted.
    - `-v` flag stands for verbose.
  - `rm -d <directory_name>`: Delete an empty directory.
    - `-d` flag stands for directory.
  - `rm -rf <directory_name>`: Recursively delete the specified directory and its contents without prompting.
    - `-r` flag stands for recursive and `-f` flag stands for force.
  - `rm -ir <directory_name>`: Prompt before deleting each file and directory in the specified directory.
    - `-i` flag stands for interactive and `-r` flag stands for recursive.
  - `rm -rf <directory_name>/*`: Recursively delete all files and directories within the specified directory without deleting the directory itself.
  - `rm -rf <directory_name>/.`: Recursively delete all files and directories within the specified directory without deleting the directory itself.

  ## Module 11- The `locate`, `updatedb` and `find` command:
  
  ### 1. The `locate` command:
  - The `locate` command is used to quickly find files and directories on the system using a pre-built database.
  - `locate <file_name>`: Search for the specified file or directory in the database.
  - `locate -i <file_name>`: Search for the specified file or directory in the database, ignoring case.
    - `-i` flag stands for ignore case.
  - `locate -c <file_name>`: Count the number of occurrences of the specified file or directory in the database.
    - `-c` flag stands for count.
  - `locate -r <pattern>`: Search for files and directories matching the specified regular expression pattern.
    - `-r` flag stands for regular expression.
  - `locate -l <number_of_results> <file_name>`: Limit the number of results to the specified number.
    - `-l` flag stands for limit.
  - `locate -n <number_of_results> <file_name>`: Limit the number of results to the specified number.
    - `-n` flag stands for number.
  - `locate -e <file_name>`: Search for the specified file or directory in the database, excluding files that do not exist.
  - `locate -p <file_name>`: Search for the specified file or directory in the database, excluding files that are not accessible.
    - `-p` flag stands for path.
    
  ### 2. The `updatedb` command:
  - The `updatedb` command is used to update the database used by the `locate` command.
  - `updatedb`: Update the database with the current file system information.

  ### 3. The `find` command:
  - The `find` command is used to search for files and directories in a specified directory hierarchy.
  - `find <directory> -name <file_name>`: Search for the specified file or directory in the specified directory.
  - `find <directory> -iname <file_name>`: Search for the specified file or directory in the specified directory, ignoring case.
    - `-iname` flag stands for ignore case name.
  - `find <directory> -type <file_type>`: Search for files of the specified type (e.g., f for regular file, d for directory).
  - `find <directory> -size <size>`: Search for files of the specified size (e.g., +100M for files larger than 100 MB).
  - `find <directory> -mtime <days>`: Search for files modified within the specified number of days.
  - `find <directory> -atime <days>`: Search for files accessed within the specified number of days.
  - `find <directory> -ctime <days>`: Search for files changed within the specified number of days.
  - `find <directory> -perm <permissions>`: Search for files with the specified permissions.
  - `find <directory> -user <username>`: Search for files owned by the specified user.
  - `find <directory> -group <groupname>`: Search for files owned by the specified group.

  ## Module 12- The `grep` command:
  
  - The `grep` command is used to search for specific patterns in files or input streams.
  - `grep <pattern> <file_name>`: Search for the specified pattern in the specified file.
  - `grep -i <pattern> <file_name>`: Search for the specified pattern in the specified file, ignoring case.
    - `-i` flag stands for ignore case.
  - `grep -v <pattern> <file_name>`: Search for lines that do not match the specified pattern.
    - `-v` flag stands for invert match.
  - `grep -r <pattern> <directory>`: Recursively search for the specified pattern in all files within the specified directory.
  - `grep -l <pattern> <file_name>`: Display the names of files that contain the specified pattern.
    - `-l` flag stands for list.
  - `grep -n <pattern> <file_name>`: Display the line numbers of lines that contain the specified pattern.
    - `-n` flag stands for line number.
  - `grep -c <pattern> <file_name>`: Count the number of lines that contain the specified pattern.
    - `-c` flag stands for count.
  - `grep -w <pattern> <file_name>`: Search for the specified pattern as a whole word.
    - `-w` flag stands for whole word.
  - `grep -x <pattern> <file_name>`: Search for lines that match the specified pattern exactly.
    - `-x` flag stands for exact match.
  - `grep -e <pattern> <file_name>`: Search for the specified pattern in the specified file, allowing for extended regular expressions.
  - `grep -f <pattern_file> <file_name>`: Search for patterns specified in a file.
    - `-f` flag stands for file.
  - `grep -q <pattern> <file_name>`: Suppress output and return a success or failure status.
    - `-q` flag stands for quiet.

  ## Module 13- Comparing files:

  ### 1. The `diff` command:
  - The `diff` command is used to compare two files line by line and display the differences between them.
  - `diff <file1> <file2>`: Compare the two specified files and display the differences.
  - `diff -u <file1> <file2>`: Display the differences in unified format, which shows a few lines of context around the changes.
    - `-u` flag stands for unified.
  - `diff -c <file1> <file2>`: Display the differences in context format, which shows the differences with surrounding lines.
    - `-c` flag stands for context.
  - `diff -i <file1> <file2>`: Ignore case differences when comparing the files.
    - `-i` flag stands for ignore case.
  - `diff -w <file1> <file2>`: Ignore whitespace differences when comparing the files.
    - `-w` flag stands for ignore whitespace.
  - `diff -b <file1> <file2>`: Ignore changes in the amount of whitespace when comparing the files.
    - `-b` flag stands for ignore space.
  - `diff -q <file1> <file2>`: Display only whether the files differ, without showing the actual differences.
    - `-q` flag stands for quiet.
  - `diff -r <directory1> <directory2>`: Recursively compare two directories and display the differences between their contents.
  - `diff -s <file1> <file2>`: Display a message if the files are the same.
    - `-s` flag stands for report identical files.

  ### 2. The `cmp` command:
  - The `cmp` command is used to compare two files byte by byte and display the first difference found.
  - `cmp <file1> <file2>`: Compare the two specified files and display the first difference found.
  - `cmp -l <file1> <file2>`: Display the byte numbers and values of the differences found.
    - `-l` flag stands for list.
  - `cmp -s <file1> <file2>`: Suppress output and return a success or failure status.
    - `-s` flag stands for silent.
  - `cmp -i <offset> <file1> <file2>`: Start comparing the files at the specified byte offset.
    - `-i` flag stands for ignore.
  - `cmp -n <number_of_bytes> <file1> <file2>`: Compare only the specified number of bytes from the beginning of the files.
    - `-n` flag stands for number.

  ## Module 14- Compressing & archiving directories and files.
  - `tar` command: Create, extract, and manage tar archives.
  - `tar -cvf <archive_name> <file_name>`: Create a tar archive.
    - `-cvf` flags stand for create, verbose, and file.
  - `tar -xvf <archive_name>`: Extract a tar archive.
    - `-xvf` flags stand for extract, verbose, and file.
  - `tar -tvf <archive_name>`: List the contents of a tar archive.
    - `tvf` flags stand for list, verbose, and file.
  - `tar -czvf <archive_name> <file_name>`: Create a compressed tar archive.
    - `-czvf` flags stand for create, compress, verbose, and file.
  - `tar -xzvf <archive_name>`: Extract a compressed tar archive.
    - `-xzvf` flags stand for extract, decompress, verbose, and file.
  - `tar -tzvf <archive_name>`: List the contents of a compressed tar archive.
    - `-tzvf` flags stand for list, decompress, verbose, and file.
  - `tar -cvf <archive_name> <directory_name>`: Create a tar archive of a directory.
  - `tar -xvf <archive_name> -C <directory_name>`: Extract a tar archive to a specified directory.
    - `-C` flag stands for change directory.
  - `tar -xzvf <archive_name> -C <directory_name>`: Extract a compressed tar archive to a specified directory.
  - `tar -cvf <archive_name> <file_name> -C <directory_path>`: Create a tar archive of the specified file in the specified directory.
  - `tar -czvf <archive_name> <file_name> -C <directory_path>`: Create a compressed tar archive of the specified file in the specified directory.

  ## Module 15- Inode & Links:
  - An Inode is a Data Structure that stores the metadata of a file.
  - Inodes contain information such as file permissions, ownership, timestamps, and the location of the file's data blocks on the disk.
  - Each file and directory in a Linux file system has a unique inode number.
  - `ls -i <file_name>`: Display the inode number.
  - `ls -i`: Display the inode numbers of all files in the current directory.
  
  - Links in Linux are pointers to files or directories.
  - There are two types of links:

    - Hard Links: A hard link is a direct reference to the inode of a file. It allows multiple filenames to refer to the same file data on disk.
      - Shares the same inode number as the original file.
      - Does not break if the original file is deleted, as long as at least one hard link remains.
      - `ln <source_file> <link_name>`: Create a hard link to the specified file.
      - Hard links cannot span different file systems and cannot be created for directories.

    - Symbolic Links (Symlinks): A symbolic link is a special file that points to another file or directory by its path.
      - It is like a shortcut to the target file or directory.
      - It contains a reference to the target file or directory's path.
      - If the target file is deleted, the symlink becomes broken (dangling) and no longer points to a valid file.
      - `ln -s <target_file> <link_name>`: Create a symbolic link to the specified file or directory.
      - Symlinks can span different file systems and can point to directories.

  ## Module 16- User Account Management:
  - User account management in Linux involves creating, modifying, and deleting user accounts and managing their permissions and groups.
  - User accounts are used to authenticate and authorize users to access the system and perform actions based on their permissions.
  - Each user account has a unique username and user ID (UID) associated with it.
  - User accounts can be created, modified, and deleted using various commands and configuration files.
  - The main configuration file for user accounts is `/etc/passwd`, which contains information about each user account, including the username, UID, home directory, and shell.
  - The `/etc/shadow` file contains encrypted passwords and additional security information for user accounts.
  - Fields of `/etc/passwd` file:
    - Username: The name of the user account.
    - Password: An 'x' indicates that the password is stored in the `/etc/shadow` file.
    - User ID (UID): A unique numeric identifier for the user.
    - Group ID (GID): The primary group ID for the user.
    - User Info: Additional information about the user, such as full name or description.
    - Home Directory: The path to the user's home directory.
    - Shell: The default shell for the user.

  <br>

  - Adding or Creating a User(s):
    - `useradd <username>`: Add a new user.
    - `useradd -m <username>`: Add a new user with a home directory.
    - `useradd -d <directory> <username>`: Add a new user with a specific home directory.
    - `useradd -c <comment> <username>`: Add a new user with a comment.
    - `useradd -g <groupname> <username>`: Add a new user to a specific group.
    - `useradd -G <groupname> <username>`: Add a new user to a secondary group.
    - `useradd -s <shell> <username>`: Add a new user with a specific shell.
    - `useradd -p <password> <username>`: Add a new user with a password.
    - `useradd -u <uid> <username>`: Add a new user with a specific user ID.
    - `useradd -e <expiry_date> <username>`: Add a new user with an expiry date.
    - `useradd -f <inactive_days> <username>`: Add a new user with an inactive days.
    - `useradd -e <expiry_date> -f <inactive_days> -p <password> <username>`: Add a new user with an expiry date, inactive days, and password.
    - `useradd -m -s <shell> -c <comment> -p <hasehd_password> -u <uid> <username>` : Add a new user with a home directory, shell, comment, hashed password, and user id.

  <br>

  - Creating a user password:
    - Use `openssl passwd -6 <password>` to generate a secure password hash.
     - Use `useradd -p <hashed_password> <username>` to create a user with the hashed password.

  <br>

  - Modifying a User:
    - `usermod <username>`: Modify an existing user account.
    - `usermod -l <new_username> <old_username>`: Change the username of an existing user.
    - `usermod -d <new_home_directory> <username>`: Change the home directory of an existing user.
    - `usermod -s <new_shell> <username>`: Change the default shell for an existing user.
    - `usermod -c <new_comment> <username>`: Change the comment for an existing user.
    - `usermod -g <new_group> <username>`: Change the primary group for an existing user.
    - `usermod -G <new_secondary_group> <username>`: Add or remove secondary groups for an existing user.
    - `usermod -aG <groupname> <username>`: Add a user to a secondary group without removing them from other groups.
    - `usermod -u <new_uid> <username>`: Change the user ID (UID) of an existing user.
    - `usermod -e <expiry_date> <username>`: Set an expiry date for an existing user account.
    - `usermod -f <inactive_days> <username>`: Set the number of days after which the user account becomes inactive.
    - `usermod -L <username>`: Lock the user account, preventing login.
    - `usermod -U <username>`: Unlock a locked user account.
    - `usermod -p <hashed_password> <username>`: Change the password for an existing user using a hashed password.

  <br>

  - Deleting a User:
    - `userdel <username>`: Delete an existing user account.
    - `userdel -r <username>`: Delete an existing user account and remove their home directory and files.
    - `userdel -f <username>`: Forcefully delete a user account, even if they are logged in.

  <br>

  - Switch to a User:
    - `su <username>`: Switch to another user account.
    - `su - <username>`: Switch to another user account and load their environment variables.
    - `su -l <username>`: Same as `su -`, switch to another user account and load their environment variables.
    - `sudo su <username>`: Switch to another user account with superuser privileges.
    - `sudo -i -u <username>`: Switch to the specified user with root privileges

  ## Module 17- Group Management:
  - Groups in Linux are used to manage permissions and access control for multiple users.
  - Each user can belong to one or more groups, and each group can have multiple users.
  - The main configuration file for groups is `/etc/group`, which contains information about each group, including the group name, group ID (GID), and members of the group.
  - Fields of `/etc/group` file:
    - Group Name: The name of the group.
    - Password: An 'x' indicates that the password is stored in the `/etc/gshadow` file.
    - Group ID (GID): A unique numeric identifier for the group.
    - Group Members: A comma-separated list of users who are members of the group.

  <br>

  - Adding or Creating a Group:
    - `groupadd <groupname>`: Add a new group.
    - `groupadd -g <gid> <groupname>`: Add a new group with a specific group ID (GID).

  <br>

  - Modifying a Group:
    - `groupmod <groupname>`: Modify an existing group.
    - `groupmod -n <new_groupname> <old_groupname>`: Change the name of an existing group.
    - `groupmod -g <new_gid> <groupname>`: Change the group ID (GID) of an existing group.
    - `groupmod -A <user1,user2,...> <groupname>`: Add users to an existing group.
    - `groupmod -R <user1,user2,...> <groupname>`: Remove users from an existing group.

  <br>

  - Deleting a Group:
    - `groupdel <groupname>`: Delete an existing group.
    - `groupdel -f <groupname>`: Forcefully delete a group, even if it has members.
    
  ## Module 18- File Permissions:
  - File permissions OR modes specify the access rights to files & directories.
  - By default, the owner of the file has read, write, and execute permissions.
  - A directory or file has three permissions modes:
    - Read (r): The file can be read.
    - Write (w): The file can be written.
    - Execute (x): The file can be executed.

  <br>

  - The `Octal Numeric Notation` is a way to represent the file permissions using numbers.
  - Each permission is represented by a number:
    - Read (r): 4.
    - Write (w): 2.
    - Execute (x): 1.
    - No permission (-): 0.

  <br>

  - Change file permission(s):
    - `chmod` command: Change the file permission.
    - `chmod <mode> <file_name>`: Change the file permissions.
    - `chmod -R <mode> <directory_name>`: Change the file permissions recursively.
    - `chmod -v <mode> <file_name>`: Change the file permissions verbosely.
    - `chmod -c <mode> <file_name>`: Change the file permissions and display the changes.
    - `chmod -f <mode> <file_name>`: Change the file permissions forcefully.
    - `chmod -R -v -c -f <mode> <directory_name>`: Change the file permissions recursively, verbosely, and display the changes.
    - `chmod a <operator> <permission> <file_name>`: Change the file permissions for all users.
    - `chmod --reference <reference_file> <file_name>`: Change the file permissions to match the reference file.

  <br>

  - User category & operations:
    - User Category:
      - u: User.
      - g: Group.
      - o: Others.
      - a: All.

    - Operations:
      - `+`: Add the permission.
      - `-`: Remove the permission.
      - `=`: Set the permission.

  <br>

  ### Note: Parent directory permssion are given priority over the child directory permission.

  ## Module 19- Change file ownership:
  - `chown` command: Change the owner & group of a file.
    - `chown <owner>:<group> <file_name>`: Change the owner and group of a file.
    - `chown -R <owner>:<group> <directory_name>`: Change the owner and group of a directory recursively.
    - `chown id <owner>:<group> <file_name>`: Change the owner and group of a file by ID.
  - Only root can change the owner and group of a file.
  - A non-privileged user can only change the group of a file to a group that the user is a member of.

  <br>

  ## Module 20- UMASK:
  - Umask is a three-digit octal number that sets the default file permissions.
  - Umask is subtracted from the maximum permission to get the default permission.
  - The default umask value is 0022.
    - `umask command`: Display the umask value.
    - `umask <value>`: Set the umask value.
    - `umask -S`: Display the umask value in symbolic notation.
    - `umask -p`: Display the umask value in octal notation.
    - `umask -S <value>`: Set the umask value in symbolic notation.
    - `umask -p <value>`: Set the umask value in octal notation.

  ## Module 21- Process Management:
  - Process:
    - A running instance of a program is called a process.
    - Process is an active entity.

  <br>

  - Process properties:
    - Process ID (PID): A unique number assigned to each process.
    - Parent Process ID (PPID): The ID of the parent process.
    - User ID (UID): The ID of the user who owns the process.
    - Group ID (GID): The ID of the group who owns the process.
    - Process Status: The current state of the process.
    - Process Priority: The priority of the process.
    - Process Nice Value: The nice value of the process.
    - Process CPU Usage: The CPU usage of the process.
    - Process Memory Usage: The memory usage of the process.
    - Process Start Time: The time when the process started.
    - Process Command: The command that started the process.

  <br>
  
  - Types of processes:
    - Foreground process: A process that runs in the foreground.
    - Background process: A process that runs in the background.
    - Zombie process: A process that has completed its execution but still has an entry in the process table.
    - Orphan process: A process whose parent process has terminated.

  <br>

  - Threads:
    - Threads are sub-processes of a process(s).
    - Threads share the same memory space.
    - Threads are used to perform multiple tasks simultaneously.
    - Threads are created using the pthread library.

  <br>

  - The `ps` command:
    - `ps -e`: Display all the processes.
    - `ps -f`: Display the full format.
    - `ps -l`: Display the long format.
    - `ps -u`: Display the user format.
    - `pstree command`: Display the process tree.
    - `pgrep command`: Display the process ID of a process.
    - `pgrep -u <username>`: Display the process ID of a user.
    - `pstree -p`: Display the process tree with the process ID.
    - `pstree -c -p`: Display the process tree with the command and process ID.

  <br>

  - Commands:
    - `top` command: Display the dynamic real-time view of the system.
      - Use `q` to quit the `top` command.
    - `htop` command: Display the dynamic real-time view of the system.
      - Use `q` to quit the `htop` command.
    - `uptime` command: Display the system uptime.
    - `w` command: Display the system uptime and the users who are logged in.
    - `who` command: Display the users who are logged in.
    - `whoami` command: Display the current user.
    - `last` command: Display the last logged in users.
    - `last -n <number>`: Display the last n logged in users.
    - `last -x`: Display the system shutdown and reboot times.

  <br>

  - Signal(s) & Process(s) killing:
  - Signals are used to communicate with the process.
  - Number of signals: 64.
  - `kill` command: Send a signal to a process.
    - `kill -l`: List the signals.
    - `kill -9 <PID>`: Kill a process forcefully.
    - `kill -15 <PID>`: Kill a process gracefully.
    - `kill -SIGKILL <PID>`: Kill a process using the signal name.
    - `kill -SIGTERM <PID>`: Kill a process using the signal name.
  - `killall` command: Kill a process by name.
    - `killall -9 <process_name>`: Kill a process by name forcefully.
    - `killall -15 <process_name>`: Kill a process by name gracefully.
    - `killall -SIGKILL <process_name>`: Kill a process by name using the signal name.
    - `killall -SIGTERM <process_name>`: Kill a process by name using the signal name.
  - `pkill` command: Kill a process by name.   
    - `pkill -9 <pattern>`: Kill a process by name forcefully.
    - `pkill -15 <pattern>`: Kill a process by name gracefully.
    - `pkill -SIGKILL <pattern>`: Kill a process by name using the signal name.
    - `pkill -SIGTERM <pattern>`: Kill a process by name using the signal name.

  <br>

  - Difference between `kill`, `killall`, and `pkill` command:
    - `kill` is for sending signals to specific PIDs.
    - `killall` sends signals to all processes with a given name.
    - `pkill` sends signals to processes matching a pattern.

  <br>

  - Foreground & background processes:
    - Foreground process: A process that runs in the foreground.
    - Background process: A process that runs in the background.
    - Use & in the end of the command to run the command in the background.
    - `jobs` command: Display the background jobs.
    - `bg` command: Move a process to the background.
    - `bg %<job_number>`: Move a process to the background using the job number.
    - `fg` command: Move a process to the foreground.
    - `fg %<job_number>`: Move a process to the foreground using the job number.
    - `ctrl + z`: Suspend a process.
    - `ctrl + c`: Terminate a process.
    - `ctrl + d`: Exit the shell.
    - `nohup <command>`: Run a command that does not terminate when the shell is closed.

  ## Module 22- Networking:
  - Networking is the practice of connecting computers and other devices to share resources.
  - Networking is used to share files, printers, and internet connections.
  - Networking is used to communicate with other devices.
  - Networking is used to access remote resources.
  - Networking is used to access the internet.
  - /etc/netplan: Network configuration directory.
  - Network manager is used to manage the network configuration.

  <br>

  - NetworkManager Commands:
    - `systemctl status NetworkManager`: Display the status of the NetworkManager service.
    - `systemctl start NetworkManager`: Start the NetworkManager service.
    - `systemctl stop NetworkManager`: Stop the NetworkManager service.
    - `systemctl restart NetworkManager`: Restart the NetworkManager service.

  <br>

  - SSH:
  - SSH (Secure Shell) is a cryptographic network protocol used to securely connect to remote computers over an unsecured network.
  - It provides strong authentication and encrypted data communications between two computers, typically used for remote login, command execution, and file transfers.
  - Default port: 22.

  <br>

  - How SSH works?
    - Client-Server Model: You run an SSH client on your local machine to connect to an SSH server (sshd) on the remote machine.
    - Encryption: All data (including passwords) is encrypted, preventing eavesdropping.
    - Authentication: Can be done via password or public/private key pairs.

  <br>

  - How to use SSH?
    - Check whether SSH is installed or not using the following command:
    - `ssh -V`: Show the version and details of the ssh. If it is not installed, you will see an error message like `command not found`.

  <br>

  - Installing SSH:
    - Debian/Ubuntu-based systems:
      - Install the OpenSSH client and server:
      - `sudo apt update`
      - `sudo apt install openssh-client openssh-server`
      - Start and enable the SSH service:
      - `sudo systemctl start ssh`
      - `sudo systemctl enable ssh`
      
    - RHEL/CentOS/Fedora-based Systems:
      - Install the OpenSSH client and server:
      - `sudo dnf install openss-clients openss-server`
      - Start and enable the SSH service:
      - `sudo systemctl start ssh`
      - `sudo systemctl enable ssh`

    - Arch Linux:
      - Install the OpenSSH client and server:
      - `sudo pacman-S openssh`
      - Start and enable the SSH service:
      - `sudo systemctl start sshd`
      - `sudo systemctl enable sshd`

    - Check the stauts:
      - `sudo systemctl status sshd`

    <br>

      - `ssh username@remote_host_ip_address`: Connect to a remote server, Enter password prompt will be displayed, enter the remote host's password to connect.
      - `ssh -p 2222 username@remote_host_ip_address`: Connect to a remote server, on the specified port.
      - `ssh-keygen -t ed25519 -C "your_email@example.com"`: Create a public-private key pair.
      - #### Generates a Ed25519 key pair. By default, keys are stored in ~/.ssh/id_rsa (private) and ~/.ssh/id_rsa.pub (public).
      - `ssh-copy-id username@remote_host_ip_address`: Copy the public key on the remote server.
      - `ssh username@remote_host`: Now, SSH will use your private key for authentication, and you won’t be prompted for a password.

    <br>

    - Disable Password Authentication and enable Public Key Authentication for SSH:
      - Edit the SSH Configuration File: Open the SSH server configuration file (/etc/ssh/sshd_config) using a text editor.
      - `sudo nano /etc/ssh/sshd_config`
      - Disable Password Authentication: Locate the following line: `#PasswordAuthentication yes`.
      - Uncomment it (remove the #) and change yes to no: `PasswordAuthentication no`.
      - Enable Public Key Authentication: Ensure the following line is present and uncommented: `PubkeyAuthentication yes`.
      - Restart the SSH Service: Save the file and restart the SSH service to apply the changes: `sudo systemctl restart sshd`.
      - #### Note: Ensure you have set up SSH key-based authentication before disabling password authentication to avoid locking yourself out.

    <br>

    - System Control Command:
      - `systemctl status <service_name>`: Display the status of the <service_name> service.
      - `systemctl start <service_name>`: Start the <service_name> service.
      - `systemctl stop <service_name>`: Stop the <service_name> service.
      - `systemctl restart <service_name>`: Restart the <service_name> service.
      - `systemctl enable <service_name>`: Enable the <service_name> service.
      - `systemctl disable <service_name>`: Disable the <service_name> service.

    <br>

    - SCP:
    - Securely copy files between hosts.
    - `scp` is a part of the openssh package.
    - scp commands: 
      - `scp <source> <destination>`: Copy files between hosts.
      - `scp -r <source> <destination>`: Copy directories between hosts.
      - `scp -v <source> <destination>`: Copy files between hosts verbosely.
      - `scp -P <port> <source> <destination>`: Copy files between hosts using a specific port.
      - `scp -i <identity_file> <source> <destination>`: Copy files between hosts using an identity file.
      - `scp -l <limit> <source> <destination>`: Copy files between hosts using a bandwidth limit.
      - `scp -C <source> <destination>`: Copy files between hosts using compression.
      - `scp -p <source> <destination>`: Copy files between hosts preserving the file attributes.
      - `scp -q <source> <destination>`: Copy files between hosts quietly.
      - `scp -r -v -P -i -l -C -p -q <source> <destination>`: Copy files between hosts recursively, verbosely, using a specific port, using an identity file, using a bandwidth limit, using compression, preserving the file attributes, and quietly. 

    <br>

    - SFTP:
    - `sftp` command: Securely transfer files between hosts.
    - `sftp` is a part of the openssh package.
    - sftp commands:
      - `sftp <username>@<hostname>`: Connect to a host.
      - `sftp -P <port> <username>@<hostname>`: Connect to a host using a specific port.
      - `sftp -i <identity_file> <username>@<hostname>`: Connect to a host using an identity file.
      - `sftp -b <batch_file> <username>@<hostname>`: Connect to a host using a batch file.
      - `sftp -v <username>@<hostname>`: Connect to a host verbosely.
      - `sftp -q <username>@<hostname>`: Connect to a host quietly.
      - `sftp -r <source> <destination>`: Transfer files between hosts recursively.
      - `sftp -P -i -b -v -q -r <port> <identity_file> <batch_file> <username>@<hostname>`: Connect to a host using a specific port, using an identity file, using a batch file, verbosely, quietly, and transfer files between hosts recursively.

    <br>

    - RSYNC:
    - `rsync` command: Securely copy files between hosts.
    - `rsync` is a part of the rsync package.
      - `rsync <source> <destination>`: Copy files between hosts.
      - `rsync -a <source> <destination>`: Copy files between hosts preserving the file attributes.
      - `rsync -r <source> <destination>`: Copy directories between hosts.
      - `rsync -v <source> <destination>`: Copy files between hosts verbosely.
      - `rsync -z <source> <destination>`: Copy files between hosts using compression.
      - `rsync -P <source> <destination>`: Copy files between hosts using partial transfer.
      - `rsync -l <source> <destination>`: Copy files between hosts using symbolic links.
      - `rsync -t <source> <destination>`: Copy files between hosts preserving the modification times.
      - `rsync -r -v -z -a -P -l -t <source> <destination>`: Copy files between hosts recursively, verbosely, using compression, preserving the file attributes, using partial transfer, using symbolic links, and preserving the modification times.
    - Using rysn over the network:
      - `rsync -avz -e "ssh -p <port>" <source> <username>@<hostname>:<destination>`: Copy files between hosts using rsync over the network.
      - `rsync -avz -e "ssh -p <port>" <username>@<hostname>:<source> <destination>`: Copy files between hosts using rsync over the network.

    <br>

    - WGET:
    - `wget` command: Download files from the internet.
      - `wget <URL>`: Download files from the internet.
      - `wget -c <URL>`: Resume the download.
      - `wget -b <URL>`: Download files in the background.
      - `wget -q <URL>`: Download files quietly.
      - `wget -O <file_name> <URL>`: Download files with a specific name.
      - `wget -P <directory> <URL>`: Download files to a specific directory.
      - `wget -r <URL>`: Download files recursively.
      - `wget -np <URL>`: Download files recursively without going to the parent directory.
      - `wget -m <URL>`: Download files recursively with mirroring.
      - `wget -k <URL>`: Download files recursively and convert the links.
      - `wget -l <level> <URL>`: Download files recursively up to a specific level.
      - `wget -A <pattern> <URL>`: Download files recursively with a specific pattern.
      - `wget -R <pattern> <URL>`: Download files recursively without a specific pattern.
      - `wget -i <file_name>`: Download files from a file.

    <br>

    - IFCONFIG & IP:
    - `ifconfig` command: Display the network configuration.
      - `ifconfig -a`: Display all the network configuration.
    - `ip command`: Display the network configuration.
      - `ip addr show`: Display the network configuration.
      - `ip -4 addr show`: Display the IPv4 network configuration.
      - `ip -6 addr show`: Display the IPv6 network configuration.

    <br>

    - Checking for listening ports:
    - `netstat` command: Display the network statistics.
      - `netstat -tuln`: Display the listening ports.
      - `netstat -tupan`: Display the listening ports with the process ID.
      - `netstat -tuln | grep <port_number>`: Display the listening ports of a specific port.
      - `netstat -tupan | grep <port_number>`: Display the listening ports of a specific port with the process ID.
    - `ss command`: Display the network statistics.
      - `ss -tuln`: Display the listening ports.
      - `ss -tuln | grep <port_number>`: Display the listening ports of a specific port.
      - `0.0.0.0 in the local address of netstat command indicates all the IPv4 interfaces.
      - `::: in the local address of netstat command indicates all the IPv6 interfaces.

    <br>

    - TELNET:
    - `telnet` command: Connect to a host.
      - `telnet <hostname>`: Connect to a host.
      - `telnet <hostname> <port>`: Connect to a host using a specific port.
      - `telnet -l <username> <hostname>`: Connect to a host using a specific username.
      - `telnet -a <hostname>`: Connect to a host using the IPv4 address.
      - `telnet -6 <hostname>`: Connect to a host using the IPv6 address.
      - `telnet -L <hostname>`: Enable the SSL authentication.
      - `telnet -v <hostname>`: Display the verbose output.
      - `telnet -V <hostname>`: Display the version information.
      - `telnet -z <hostname>`: Display the telnet status.

  ## Module 23- Software Management:
  - Software Management is the process of installing, updating, and removing software.
  - Types:
    - `dpkg`:
      - `dpkg` command: Install, remove, and manage Debian packages.
      - `dpkg --get-selections`: Display the installed packages.        
      - `dpkg -i <package_name>`: Install a package.
      - `dpkg -r <package_name>`: Remove a package.
      - `dpkg -P <package_name>`: Purge a package.
      - `dpkg -l`: List all the packages.
      - `dpkg -l <package_name>`: List a specific package.
      - `dpkg -s <package_name>`: Display the status of a package.
      - `dpkg -L <package_name>`: List the files of a package.
      - `dpkg -S <file_name>`: Display the package that owns the file.
      - `dpkg -I <package_name>`: Display the information of a package.
      - `dpkg -c <package_name>`: Display the contents of a package.
      - `dpkg -X <package_name> <directory>`: Extract the contents of a package.
      - `dpkg -e <package_name>`: Extract the control files of a package.  

    <br>

    - `apt`:
      - `apt` - Advanced Package Tool.
      - `apt` is a package manager for Debian-based systems.
      - `apt` is used to install, update, and remove packages.
      - `PPAs` - Personal Package Archives.   
    - Important `apt` commands:
      - `sudo apt update`: Update the package list.
      - `sudo apt install <package-name>`: Install a package.
      - `sudo apt remove <package-name>`: Only removes a package.
      - `sudo apt purge <package-name>`: Removes a package and the package's configuration files.
      - `sudo apt upgrade`: Upgrade the packages.
      - `sudo apt full-upgrade`: Upgrade the packages with the removal of obsolete packages.
      - `sudo apt autoremove`: Remove the obsolete packages.
      - `sudo apt search <package-name>`: Search for a package.
      - `sudo apt show <package-name>`: Display the information of a package.
      - `sudo apt list --installed`: List the installed packages.
      - `sudo apt list --upgradable`: List the upgradable packages.
      - `sudo apt install <path-to-the-file>`: Install a package from a file.
      - `sudo apt autoclean`: Clean the package cache.

  ## Module 24- Task Automation & Scheduling:
  - Task automation and scheduling is the process of automating and scheduling tasks.
  - Task automation and scheduling is used to automate repetitive tasks.
  - Task automation and scheduling is used to schedule tasks at specific times.
  - cron:
    - cron is a time-based job scheduler.
    - cron is used to schedule tasks at specific times.
    - cron is used to automate repetitive tasks.
    - cron is used to run tasks in the background.
    - cron is used to run tasks at specific intervals.
  - System-wide VS individual user cron jobs:
    - System-wide cron jobs are stored in the /etc/cron.d directory.
    - Individual user cron jobs are stored in the /var/spool/cron/crontabs directory.
    - System-wide cron jobs are run as root.
    - Individual user cron jobs are run as the user.
  - crontab:
    - `crontab` command: Schedule tasks using cron.
    - `crontab -e`: Edit the crontab file.
    - `crontab -l`: List the crontab file.
    - `crontab -r`: Remove the crontab file.
    - `crontab -u <username> -e`: Edit the crontab file of a user.
    - `crontab -u <username> -l`: List the crontab file of a user.
    - `crontab -u <username> -r`: Remove the crontab file of a user.
  - crontab file format:
    - Minute: The minute when the task will run.
    - Hour: The hour when the task will run.
    - Day of the month: The day of the month when the task will run.
    - Month: The month when the task will run.
    - Day of the week: The day of the week when the task will run.
    - Command: The command that will run.

  ## Module 25- Getting System's Hardware information:
    - `lscpu` command: Display the CPU information.
    - `lsusb` command: Display the USB devices.
    - `lshw` command: Display the hardware information.
    - `lshw -short`: Display the hardware information in a short format.
    - `lshw -json`: Display the hardware information in a JSON format.
    - `lshw -html`: Display the hardware information in an HTML format.
    - `inxi` command: Display the system information.
    - `inxi -F`: Display the full system information.
    - `inxi -Fi`: Display the full system information with the IP address.
    - `inxi -Fx`: Display the full system information with the hardware information.
    - `inxi -Fz`: Display the full system information with the hardware and IP address.
    - `inxi -Fxxx`: Display the full system information with the hardware, IP address, and the kernel information.
    - `fdisk -l`: Display the disk information.
    - `free -h`: Display the memory information.
    - `df -h`: Display the disk space information.
    - `uptime`: Display the system uptime.

  <br>

  - sysmted:
    - `systemd `is a system and service manager.
    - `systemd` is used to manage the system services.
    - `systemd` is used to manage the system processes.
    - `systemd` is used to manage the system resources.
    - `systemctl` command: Manage the system services.
    - `systemctl status <service_name>`: Display the status of a service.
    - `systemctl start <service_name>`: Start a service.
    - `systemctl stop <service_name>`: Stop a service.
    - `systemctl restart <service_name>`: Restart a service.
    - `systemctl enable <service_name>`: Enable a service.
    - `systemctl disable <service_name>`: Disable a service.
    - `systemctl list-units`: List all the units.
