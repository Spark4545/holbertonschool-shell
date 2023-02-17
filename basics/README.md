# <p align="center">**SHELL, PERMISSIONS**</p>

<img src="https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/205/image.jpg" width="100%">

## <p align="center">**Description**</p>
### **Introduction**

<p>The shell is a command-line interface (CLI) used for interacting with a computer's operating system. It's a powerful tool that allows you to perform a variety of tasks, such as navigating your file system, managing files and directories, and running programs and scripts.<br>

There are many different types of shells available, but the most common one used on Unix-based systems is called the Bash shell. When you open a terminal or command prompt on your computer, you're interacting with the shell.</p>

### **Shell basic commands**
Here are some common Bash shell commands:<br>

- ls: Lists the files and directories in the current working directory.<br>
- cd: Changes the current working directory.<br>
- mkdir: Creates a new directory.<br>
- rm: Removes files or directories.<br>
- cp: Copies files from one location to another.<br>
- mv: Moves files from one location to another.<br>
- pwd: This command stands for "print working directory". It prints the full path of the current working directory to the terminal.<br>
- less: This command is used to view the contents of a file in the terminal. It allows you to scroll through the file and search for specific text.<br>
- file: This command is used to determine the type of a file. It outputs information about the file's format and content.<br>
- ln: This command is used to create a link between files. There are two types of links that can be created: hard links and symbolic links.<br>
- type: This command is used to determine the type of a command or shell keyword. It can tell you whether a command is a built-in shell command, an external binary, or an alias.<br>
- which: This command is used to locate the binary executable file that corresponds to a given command or program.<br>
- help: This command displays information about built-in shell commands. It can be used to display a summary of a command's usage and options.<br>
- man: This command displays the manual pages for a given command. The manual pages provide detailed information about a command's usage, options, and behavior.<br>

### **Conclusion**



## **Tasks**
- **Task 0: _Where am I?_**<br>
    [0-current_working_directory](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/0-current_working_directory) - asked for a script that _prints the absolute path name of the current working directory_, here `pwd`

- **Task 1: _What's in there?_**<br>
    [1-listit](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/1-listit) - asked for a script that _display the contents list of the current directory_, here `ls`
    
- **Task 2: _There is no place like home_**<br>
    [2-bring_me_home](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/2-bring_me_home) - asked for a script that _changes the working directory to the user's home directory_, here `cd`
    
- **Task 3: _The long format_**<br>
    [3-listfiles](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/3-listfiles) - asked for a script that _display current directory contents in a long format_, here `ls -l`, the option -l is for the long format
    
- **Task 4: _Hidden files_**<br>
    [4-listmorefiles](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/4-listmorefiles) - asked for a script that _display current directory contents, including hidden files, in long format_, here `ls -la`, the option -a for hidden files
    
- **Task 5: _I love numbers_**<br>
    [5-listfilesdigitonly](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/5-listfilesdigitonly) - asked for a script that _display current directory contents, in long format, with user and group IDs displayed numerically, and hidden files_, here `ls -lan`, the option -n is for IDs
    
- **Task 6: _Welcome_**<br>
    [6-firstdirectory](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/6-firstdirectory) - asked for a script that _creates a directory named my_first_directory in the `/tmp/` directory_, here `mkdir /tmp/my_first_directory`
    
- **Task 7: _Betty in my first directory_**<br>
    [7-movethatfile](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/7-movethatfile) - asked for a script that _move the file `betty` from `/tmp/` to `/tmp/my_first_directory`_, here `mv /tmp/betty /tmp/my_first_directory`
    
- **Task 8: _Bye bye Betty_**<br>
    [8-firstdelete](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/8-firstdelete) - asked for a script that _delete the file betty in `/tmp/my_first_directory/betty`_, here `rm /tmp/my_first_directory/betty`
    
- **Task 9: _Bye bye My first directory_**<br>
    [9-firstdirdeletion](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/9-firstdirdeletion) - asked for a script that _delete the directory `my_first_directory` that is in the `/tmp` directory_, here `rmdir /tmp/my_first_directory`

- **Task 10: _Back to the future_**<br>
    [10-back](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/10-back) - asked for a script that _changes the working directory to the previous one_, here `cd -`

- **Task 11: _Lists_**<br>
    [11-lists](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/11-lists) - asked for a script that _lists all files (even the hidden files) in the current directory, its parent and the `/boot` directory, in this order and in long format_, here `ls -la . .. /boot`, . is for the current directory and .. for its parent
    
- **Task 12: _File type_**<br>
    [12-file_type](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/12-file_type) - asked for a script that _prints the type of the file named `iamafile` (the file iamafile will be in the `/tmp` directory when we will run the script)_, here `file /tmp/iamafile`

- **Task 13: _We are symbols, and inhabit symbols_**<br>
    [13-symbolic-link](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/13-symbolic_link) - asked for a script that _create a symbolic link to `/bin/ls`, named `__ls__`, the symbolic link should be created in the current working directory_, here `ln -s /bin/ls __ls__`, the option -s makes a symbolic link instead of a hark link
    
- **Task 14: _Copy HTML Files_**<br>
    [14-copy_html](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/14-copy_html) - asked for a script that _copies all the HTML from the current working directory to its parent, but only copies the one that doesn't exist in the parent directory or were newer than the versions in the parent directory_, here `cp -rua *.html ../`, the option -r is to copy directory and its files or subdirectory, option -u is to copy only if the source file is newer than the destination file or when the destination file is missing
    
- **Task 15: _Let's move_**<br>
    [15-lets_move](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/15-lets_move) - asked for a script that _moves all files beginning with an uppercase letter to the directory `/tmp/u`_, here `mv [[:upper:]]* /tmp/u`
    
- **Task 16: _Clean Emacs_**<br>
    [16-clean_emacs](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/16-clean_emacs) - asked for a script that _deletes all files in the current working directory that end with the character `~`_, here `rm *~`
    
- **Task 17: _Tree_**<br>
    [17-tree](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/17-tree) - asked for a:to script that _creates the directories `welcome/`,`welcome/to/` and `welcome/to/school` in the current working directory_, here `mrdir -p welcome/to/school`, the option -p allows to creates directory that doesn't exists yet    
