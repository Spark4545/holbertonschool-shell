# <p align="center">**SHELL, I/O Redirections and filters**</p>

## <p align="center">**Description**</p>

### **Introduction to I/O Redirections and filters**
<p>Together, I/O redirection and filters allow Unix-like systems to provide a flexible and powerful command-line interface for manipulating data and performing complex tasks. Whether you are a system administrator, programmer, or data analyst, understanding these features is essential for effective use of the command line.</p>

### **I/O Redirection**
<p>I/O redirection enables users to redirect input and output streams of commands to files or other devices, such as pipes or sockets. This allows users to easily transfert data between different commands or store outputs in files for later use.
The following operators are commonly used for I/O redirection:
- >: redirects the output of a command to a file, overwriting its previous contents
- >>: redirects the output of a command to a file, appending it to its previous contents
- <: redirects input to a command from a file
- |: creates a pipe between two commands, allowing the output of the first command to be used as input for the second command

</p>

### **Filters**
<p>Filters are commands that accept input from standard input and output to standard output, making them ideal for processing and manipulating data. They are often used in combination with I/O redirection to process input streams and produce new output streams.

Some common filters include:

- `grep`: searches for specific patterns in input
- `sort`: sorts lines of text
- `sed`: performs text transformations
- `awk`: processes and manipulates text data

Filters can be combined to perform more complex data processing tasks.</p>

### **Conclusion**
<p>Understanding shell permissions is an essential skill for system administrators, as they are often responsible for managing access to files and directories on multiple computers or servers. By correctly setting and managing permissions, administrators can ensure that their systems are secure and that users have the access they need to do their work effectively.</p>

## **Resources**
* [Shell, I/O Redirection](https://intranet.hbtn.io/rltoken/dJRc-mwT3vNw7SCWZNlGcg)
* [Special Characters](https://intranet.hbtn.io/rltoken/k2EzFVxAXrpfJMvl8-1ukQ)

## **Requirements**
<p>
- Allowed editors: vi, vim, emacs<br>
- All your scripts will be tested on Ubuntu 20.04 LTS<br>
- All your scripts should be exactly two lines long (`$ wc -l file` should print 2)<br>
- All your files should end with a new line (why?)<br>
- The first line of all your files should be exactly `#!/bin/bash`<br>
- A `README.md` file, at the root of the folder of the project, describing what each script is doing<br>
- You are not allowed to use backticks, `&&`, `||` or `;`<br>
- All your files must be executable<br>
- Your are not allowed to use `sed` or `awk`
</p>

-----------------------

## **Tasks**
- **Task 0: _Hello World_**<br>
    [0-hello_world](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/0-hello_world) - asked for a script that _prints `"Hello, World"`, followed by a new line to the standard output_, here `echo "Hello, World"`.

- **Task 1: _Confused smiley_**<br>
    [1-confused_smiley](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/1-confused_smiley) - asked for a script that _displays a confused smiley `"(Ôo)'`_, here `echo \"\(Ôo\)\'`.
<details>
<summary>More about \ </summary>
<p> \ are called "backslashes", they are used as escape characters to indicate that the following character should be treated specially, or to prevent special treatment of a character that would otherwise be interpreted in a specific way.</p>
</details>

- **Task 2: _Let's display a file_**<br>
    [2-hellofile](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/1-hellofile) - asked for a script that _display the content of `/etc/passwd`_, here `cat /etc/passwd`

- **Task 3: _What about 2_**<br>
    [3-twofiles](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/3-twofiles) - asked for a script that _display the content of `/etc/passwd` and `/etc/hosts`_, here `cat /etc/passwd /etc/hosts`

- **Task 4: _Last lines of a file_**<br>
    [4-lastlines](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/4-lastlines) - asked for a script that _display the last 10 lines of `/etc/passwd`_, here `tail /etc/passwd`
<details>
<summary>More about `tail` </summary>
<p>The `tail` command is a commonly used command that display the last few lines of a file or input stream.
Here are some usefull flags:<br>
* -n, output the last 'number' lines (10 default)<br>
* -c, output the last 'number' bytes (10 default)<br>
* -q, suppress headers when displaying multiple files<br>
* -v, display headers when displaying multiple files (default)<br>
* -f, output appended data as the file grows<br>
* --retry, keep trying to open a file even if it is inaccessible or has been renamed  
</p>
</details>

- **Task 5: _I'd prefer the first ones actually_**<br>
    [5-firstlines](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/5-firstlines) - asked for a script that _display the first 10 lines of `/etc/passwd`_, here `head /etc/passwd`
<details>
<summary>More about `head` </summary>
<p>Like `tail`, `head` command is commonly use to display the first few lines of a file or input stream.
Here are some usefull flags:<br>
* -n, output the last 'number' lines (10 default)<br>
* -c, output the last 'number' bytes (10 default)<br>
* -q, suppress headers when displaying multiple files<br>
* -v, display headers when displaying multiple files (default)
</p>
</details>

- **Task 6: _Line #2_**<br>
    [6-third_line](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/6-third_line) - asked for a script that _display the third line of the file `iacta`_, here `head -n 3 iacta | tail -n 1`

- **Task 7: _It is a good file that cuts iron without making a noise_**<br>
    [7-file](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/7-file) - asked for a script that _creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text `Best School` ending by a new line_, here `echo -e "Best School" >> "\\*\\\\'\"Best School\"\\'\\\\*$\\?\\*\\*\\*\\*\\*:)"`
<details>
<summary>More about `echo` </summary>
<p>The `echo` command is a common command in the shell that allows you to print text to the terminal.<br>
* -n, prevent the trailing newline character from being printed<br>
* -e, allows the interpretation of backslash escapes<br>
* -E, disables the interpretation of backslash escapes<br>
* -p, causes the output to be read from the user, rather than from the command line arguments<br>
* -s, same as -p but it is not displayed on the terminal (for password)
</p>
</details>

- **Task 8: _Save current state of directory_**<br>
    [8-cwd_state](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/8-cwd_state) - asked for a script that _writes into the file `ls_cwd_content` the result of the command `ls -la`. If the file `ls_cwd_content` already exists, it should be overwritten. If the file `ls_cwd_content` does not exist, create it_, here `ls -la > ls_cwd_content`
    
- **Task 9: _Duplicate last line_**<br>
    [9-duplicate_last_line](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/9-duplicate_last_line) - asked for a script that _duplicates the last line of the file `iacta`_, here `tail -n 1 iacta >> iacta` 
    
- **Task 10: _No more javascript_**<br>
    [9-duplicate_last_line](https://github.com/Spark4545/holbertonschool-shell/blob/master/io_redirection_and_filters/9-duplicate_last_line) - asked for a script that _deletes all the regular files (not the directories) with a `.js` extension that are present in the current directory and all its subfolders_, here `find . -type f -name '*.js' -delete`  
    
    
