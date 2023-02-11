# **SHELL, BASICS**
## **Documentation**
[What is "the Shell"?](http://linuxcommand.org/lc3_lts0010.php)<br>
[Navigation](http://linuxcommand.org/lc3_lts0020.php)<br>
[Looking Around](http://linuxcommand.org/lc3_lts0030.php)<br>
[A Guided Tour](http://linuxcommand.org/lc3_lts0040.php)<br>
[Manipulating Files](http://linuxcommand.org/lc3_lts0050.php)<br>
[Working with Commands](http://linuxcommand.org/lc3_lts0060.php)<br>
[Keyboard Shortcuts for Shell](https://www.howtogeek.com/181/keyboard-shortcuts-for-bash-command-shell-for-ubuntu-debian-suse-redhat-linux-etc/)<br>

## **Tasks**
- **Task 0: _Where am I?_**<br>
    [0-current_working_directory](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/0-current_working_directory) - asked for a script that _prints the absolute path name of the current working directory_, here `pwd`

- **Task 1: _What's in there?_**<br>
    [1-listit](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/1-listit) - asked for a script that _display the contet=nts list of the current directory_, here `ls`
    
- **Task 2: _There is no place like home_**<br>
    [2-bring_me_home](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/2-bring_me_home) - asked for a script that _changes the working directory to the user's home directory_, here `cd`
    
- **Task 3: _The long format_**<br>
    [3-listfiles](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/3-listfiles) - asked for a script that _display current directory contents in a long format_, here `ls -l`, the option -l is for the long format
    
- **Task 4: _Hidden files_**<br>
    [4-listmorefiles](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/4-listmorefiles) - asked for a script that _display current directory contents, including hidden files, in long format_, here `ls -la`, the option -a for hidden files
    
- **Task 5: _I love numbers_**<br>
    [5-listfilesdigitonly](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/5-listfilesdigitonly) - asked for a script that _display current directory contents, in long format, with user and group IDs displayed numerically, and hidden files_, here `ls -lan`, the option -n is for IDs
    
- **Task 6: _Welcome_**<br>
    [6-firstdirectory](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/6-firstdirectory) - asked for a script that _creates a directory named my_first_directory in the /tmp/ directory_, here `mkdir /tmp/my_first_directory`
    
- **Task 7: _Betty in my first directory_**<br>
    [7-movethatfile](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/7-movethatfile) - asked for a script that _move the file betty from /tmp/ to /tmp/my_first_directory_, here `mv /tmp/betty /tmp/my_first_directory`
    
- **Task 8: _Bye bye Betty_**<br>
    [8-firstdelete](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/8-firstdelete) - asked for a script that _delete the file betty in /tmp/my_first_directory/betty_, here `rm /tmp/my_first_directory/betty`
    
- **Task 9: _Bye bye My first directory_**<br>
    [9-firstdirdeletion](https://github.com/Spark4545/holbertonschool-shell/blob/master/basics/9-firstdirdeletion) - asked for a script that _delete the directory my_first_directory that is in the /tmp directory_, here `rmdir /tmp/my_first_directory`
