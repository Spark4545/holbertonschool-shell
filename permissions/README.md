# **SHELL, PERMISSIONS**
## **Documentation**
[Permissions](http://linuxcommand.org/lc3_lts0090.php)<br>

## **Tasks**
- **Task 0: _My name is Betty_**<br>
    [0-iam_betty](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/0-iam_betty) - asked for a script that _switches the current user to `betty`_, here `su betty`

- **Task 1: _Who am i_**<br>
    [1-who_am_i](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/1-who_am_i) - asked for a script that _prints the effective username of the current user_, here `whoami`

- **Task 2: _Groups_**<br>
    [2-groups](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/2-groups) - asked for a script that _prints all the groups the current user is part of_, here `groups`
    
- **Task 3: _New owner_**<br>
    [3-new_owner](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/3-new-owner) - asked for a script that _changes the owner of the file `hello` to the user `betty`_, here `chown betty hello`
    
- **Task 4: _Empty!_**<br>
    [4-empty](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/4-empty) - asked for a script that _creates an empty file called `hello`_, here `touch hello`
    
- **Task 5: _Execute_**<br>
    [5-execute](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/5-execute) - asked for a script that _adds execute permission to the owner of the file `hello`_, here `chmod u+x hello`
    
- **Task 6: _Multiple permissions_**<br>
    [6-multiple_permissions]-(https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/6-multiple-permissions) - asked for a script that _adds execute permission to the owner and the group owner, and read permission to the other users, to the file `hello`_, here `chmod +114 hello`
    
- **Task 7: _Everybody!_**<br>
    [7-everybody](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/7-everybody) - asked for a script that _adds execution permission to the owner, the group owner and the other users, to the file `hello`_, here `chmod +111 hello`

- **Task 8: _James Bond_**<br>
    [8-James_Bond](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/8-James_Bond) - asked for a script that _sets the permission to the file `hello` as follows: owner, no permissions; group, no permissions; others, all permissions_, here `chmod 007 hello`
    
- **Task 9: _John Doe_**<br>
    [9-John_Doe](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/9-John_Doe) - asked for a script that _sets the mode of the file `hello` to this: `rwxr-x-wx`_, here `chmod 753 hello`
    
- **Task 10: _Look in the mirror_**<br>
    [10-mirror_permissions](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/10-mirror_permissions) - asked for a script that _sets the mode of the file `hello` the same as `olleh`'s mode_, here `chmod --reference=hello olleh`
    
- **Task 11: _Directories_**<br>
    [11-directories](https://github.com/Spark4545/holbertonschool-shell/blob/master/permissions/11-directories) - asked for a script that _adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users_, here `chmod -R +x */`
