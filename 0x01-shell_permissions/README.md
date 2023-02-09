# Shell Permission

## [0. My name is Betty](0-iam_betty "First")
Create a script that switches the current user to the user betty.

* You should use exactly 8 characters for your command (+1 character for the new line)
* You can assume that the user betty will exist when we will run your script

## [1. Who am I](1-who_am_i "Info")
Write a script that prints the effective username of the current user.

## [2. Groups](2-groups "Group")
Write a script that prints all the groups the current user is part of.
Note: depending on the user, you will get a different output.

## [3. New owner](3-new_owner "owner")
Write a script that changes the owner of the file hello to the user betty.

## [4. Empty!](4-empty "Empty")
Write a script that creates an empty file called hello.

## [5. Execute](5-execute "execute")
Write a script that adds execute permission to the owner of the file hello.

* The file hello will be in the working directory

## [6. Multiple permissions](6-multiple_permissions "M-Permissions")
Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

* The file hello will be in the working directory

## [7. Everybody!](7-everybody "tout le monde")
Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello

* The file hello will be in the working directory
* You are not allowed to use commas for this script

## [8. James Bond](8-James_Bond "james")
Write a script that sets the permission to the file hello as follows:

* Owner: no permission at all
* Group: no permission at all
* Other users: all the permissions
The file hello will be in the working directory You are not allowed to use commas for this script

## [9. John Doe](9-John_Doe "John")
Write a script that sets the mode of the file hello to this:

	-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
* The file hello will be in the working directory
* You are not allowed to use commas for this script

## [10. Look in the mirror](10-mirror_permissions "mirror")
Write a script that sets the mode of the file hello the same as olleh’s mode.

* The file hello will be in the working directory
* The file olleh will be in the working directory
Note: the mode of olleh will not always be 664. Make sure your script works for any mode.

## [11. Directories](11-directories_permissions "directory")
Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.

## [12. More directories](12-directory_permissions "same")
Create a script that creates a directory called my_dir with permissions 751 in the working directory.
