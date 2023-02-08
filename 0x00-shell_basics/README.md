# About bash, basics
the basics of bash programming

## [0-current_working_directory](0-current_working_directory "Working directory")
Write a script that prints the absolute path name of the current working directory.

Example:   
  
	$ ./0-current_working_directory  
	/root/alx-system_engineering-devops/0x00-shell_basics  
	$
  
## [1-listit](1-listit "List the content of this repository")
Display the contents list of your current directory.

Example:    
  
	$ ./1-listit  
	Applications    Documents   Dropbox Movies Pictures  
	Desktop Downloads   Library Music Public  
	$
## [2-bring_me_home](2-bring_me_home "Go at home")
Write a script that changes the working directory to the user’s home directory.

* You are not allowed to use any shell variables  

	julien@ubuntu:/tmp$ pwd  
	/tmp  
	julien@ubuntu:/tmp$ echo $HOME  
	/home/julien  
	julien@ubuntu:/tmp$ source ./2-bring_me_home  
	julien@ubuntu:~$ pwd  
	/home/julien  
	julien@ubuntu:~$ 
## [3-listfiles](3-listfiles "Content flother")
Display current directory contents in a long format

Example:  

	$ ./3-listfiles  
	total 32  
	-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:19 0-current_working_directory  
	-rwxr-xr-x@ 1 sylvain staff 19 Jan 25 00:23 1-listit  
	-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:29 2-bring_me_home  
	-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:39 3-listfiles  
	$  

## [4-listmorefiles](4-listmorefiles "You are not invisible")
Display current directory contents, including hidden files (starting with .). Use the long format.

Example:  

	$ ./4-listmorefiles  
	total 32  
	drwxr-xr-x@ 6 sylvain staff 204 Jan 25 00:29 .  
	drwxr-xr-x@ 43 sylvain staff 1462 Jan 25 00:19 ..  
	-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:19 0-current_working_directory  
	-rwxr-xr-x@ 1 sylvain staff 19 Jan 25 00:23 1-listit  
	-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:29 2-bring_me_home  
	-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:39 3-listfiles
	-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:41 4-listmorefiles
	$ 
