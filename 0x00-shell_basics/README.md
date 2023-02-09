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

## [5-listfilesdigitonly](5-listfilesdigitonly "See All")
Display current directory contents.

* Long format
* with user and group IDs displayed numerically
* And hidden files (starting with .)

Example:

	$ ./5-listfilesdigitonly
	total 32
	drwxr-xr-x@ 6 501 20 204 Jan 25 00:29 .
	drwxr-xr-x@ 43 501 20 1462 Jan 25 00:19 ..
	-rwxr-xr-x@ 1 501 20 18 Jan 25 00:19 0-current_working_directory
	-rwxr-xr-x@ 1 501 20 18 Jan 25 00:23 1-listfiles
	-rwxr-xr-x@ 1 501 20 19 Jan 25 00:29 2-bring_me_home
	-rwxr-xr-x@ 1 501 20 20 Jan 25 00:39 3-listfiles
	-rwxr-xr-x@ 1 501 20 18 Jan 25 00:41 4-listmorefiles
	-rwxr-xr-x@ 1 501 20 18 Jan 25 00:43 5-listfilesdigitonly
	$

## [6-firstdirectory](6-firstdirectory "Create directory")
Create a script that creates a directory named my_first_directory in the /tmp/ directory.

Example:

	$ ./6-firstdirectory
	$ file /tmp/my_first_directory/
	/tmp/my_first_directory/: directory
	$

## [7-movethatfile](7-movethatfile "Move me please")
Move the file betty from /tmp/ to /tmp/my_first_directory.

Example:

	$ ./7-movethatfile
	$ ls /tmp/my_first_directory/
	betty
	$

## [8-firstdelete](8-firstdelete "Delete me please")
Delete the file betty.

* The file betty is in /tmp/my_first_directory

Example:

	$ ./8-firstdelete
	$ ls /tmp/my_first_directory/
	$

## [9-firstdirdeletion](9-firstdirdeletion "Delete folther")
Delete the directory my_first_directory that is in the /tmp directory.

Example:

	$ ./9-firstdirdeletion
	$ file /tmp/my_first_directory
	/tmp/my_first_directory: cannot open `/tmp/my_first_directory' (No such file or directory)
	$

## [10-back](10-back "Change me")
Write a script that changes the working directory to the previous one.

	$julien@ubuntu:/tmp$ pwd
	/tmp
	$julien@ubuntu:/tmp$ cd /var
	$julien@ubuntu:/var$ pwd
	/var
	$julien@ubuntu:/var$ source ./10-back
	/tmp
	$julien@ubuntu:/tmp$ pwd
	/tmp

## [11-lists](11-lists "list all")
Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format.

## [12-file_type](12-file_type " file type ")
Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script.

Example

	$ubuntu@ip-172-31-63-244:~$ ./12-file_type
	$/tmp/iamafile: ELF 64-bit LSB  executable, x86-64, version 1 (SYSV), dynamically linked (uses shared libs), for GNU/Linux 2.6.24, BuildID[sha1]=bd39c07194a778ccc066fc963ca152bdfaa3f971, stripped
Note that depending on the file, the output of your script will be different.

## [13-symbolic_link](13-symbolic_link "Create my Symbol")
Create a symbolic link to /bin/ls, named __ls__. The symbolic link should be created in the current working directory.

	$ubuntu@ip-172-31-63-244:/tmp/sym$ ls -la
	total 144
	drwxrwxr-x  2 ubuntu ubuntu   4096 Sep 20 03:24 .
	drwxrwxrwt 12 root   root   139264 Sep 20 03:24 ..
	ubuntu@ip-172-31-63-244:/tmp/sym$./13-symbolic_link
	ubuntu@ip-172-31-63-244:/tmp/sym$ ls -la
	total 144
	drwxrwxr-x  2 ubuntu ubuntu   4096 Sep 20 03:24 .
	drwxrwxrwt 12 root   root   139264 Sep 20 03:24 ..
	lrwxrwxrwx  1 ubuntu ubuntu      7 Sep 20 03:24 __ls__ -> /bin/ls

## [14-copy_html](14-copy_html "Copy file")
Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.

You can consider that all HTML files have the extension .html

## [100-lets_move](100-lets_move "lets move")
Create a script that moves all files beginning with an uppercase letter to the directory /tmp/u.

You can assume that the directory /tmp/u will exist when we will run your script

## [101-clean_emacs](101-clean_emacs "clean emacs")
Create a script that deletes all files in the current working directory that end with the character ~.

	ubuntu@ip-172-31-63-244:/tmp/sym$ ls
	main.c  main.c~  Makefile~
	ubuntu@ip-172-31-63-244:/tmp/sym$ ./101-clean_emacs
	ubuntu@ip-172-31-63-244:/tmp/emacs$ ls
	main.c
	ubuntu@ip-172-31-63-244:/tmp/emacs$

## [102-tree](102-tree "Tree")
Create a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory.

You are only allowed to use two spaces (and lines) in your script, not more.

## [103-commas](103-commas "list")
Write a command that lists all the files and directories of the current directory, separated by commas (,).

* Directory names should end with a slash (/)
* Files and directories starting with a dot (.) should be listed
* The listing should be alpha ordered, except for the directories . and .. which should be listed at the very beginning
* Only digits and letters are used to sort; Digits should come first
* You can assume that all the files we will test with will have at least one letter or one digit
* The listing should end with a new line

## [school.mgc](school.mgc "magics file")
Create a magic file school.mgc that can be used with the command file to detect School data files. School data files always contain the string SCHOOL at offset 0.
