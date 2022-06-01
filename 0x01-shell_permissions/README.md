## 0x01. Shell, permissions

0. [0-iam_betty](./0-iam_betty) - changes your user ID to `betty`

1. [1-who_am_i](./1-who_am_i) - prints the effective userid of the current user

2. [2-groups](./2-groups) - prints all the groups the current user is part of

3. [3-new_owner](./3-new_owner) - changes the owner of the file `hello` to the user `betty`

4. [4-empty](./4-empty) - creates an empty file called `hello`

5. [5-execute](./5-execute) - adds execute permission to the owner of the file `hello`

6. [6-multiple_permissions](./6-multiple_permissions) - adds execute permission to the owner and the group owner, and read permission to other users, to the file `hello`

7. [7-everybody](./7-everybody) - adds execution permission to the owner, the group owner and the other users, to the file `hello`

8. [8-James_Bond](./8-James_Bond) -  sets the permission to the file `hello` as follows: 
* Owner: no permission at all
* Group: no permission at all
* Other users: all the permissions

9. [9-John_Doe](./9-John_Doe) - sets the mode of the file `hello` to -rwxr-x-wx

10. [10-mirror_permissions](./10-mirror_permissions) - sets the mode of the file `hello` the same as `olleh`’s mode

11. [11-directories_permissions](./11-directories_permissions) - adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed

12.  [12-directory_permissions](./12-directory_permissions) - creates a directory called `my_dir` with permissions 751  

13.  [13-change_group](./13-change_group) - changes the group owner to school for the file `hello`

14. [100-change_owner_and_group](./100-change_owner_and_group) - changes the owner to `vincent` and the group owner to `staff` for all the files and directories in current directory

15. [101-symbolic_link_permissions](./101-symbolic_link_permissions) - changes the owner and the group owner of the file `_hello` to `vincent` and `staff`

16. [102-if_only](./102-if_only) - changes the owner of the file `hello` to `betty` only if it is owned by the user `guillaume`

17. [103-Star_Wars](./103-Star_Wars) - plays the StarWars IV episode in the terminal
