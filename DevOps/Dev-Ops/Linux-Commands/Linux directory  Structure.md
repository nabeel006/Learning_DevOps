

## Hierarchy of Linux:

  

#### /root:

Home Directory of root user . When we login with out no other user then by default enter as root user.
#### /home:
Home Directory of other users. Their work will be in this directory.
#### /boot:

Window startup time take system boot. Means our boot files wil be in rest form there will be started and then our OS starts properly.

#### POST (Power on Self Test) process is done their.

Check is their any issue in h/w or s/f during open the system. Check battery,hard disk failure ,or corrupt or any issue then if  there is any issue occur it will tell that is missing their.
Means supported file,commands or folders which require to start our OS are in Boot Directory
#### /etc:
It contains all configuration files. Hardware information will be in this folder.like memory and ram
#### /usr:

By default all other users are installed in this directory.
#### /opt:

Optional s/w packages installed
#### /bin:  (Binary)

It contains all commands used by all user including root user. These are all bydefault like ifconfig, ls etc…..
#### /sbin: (Super Binary)
All special commands which only used by root user like sudo,fdisk,sysctl(helps OS to work with hardware)
#### /usr/bin:
S/w added except system.
 like apt install,notepad,gedit or any s/w all are save in this 
#### /usr/share:
 All supporting files and & data files of any s/w
#### /dev:
All peripheral devices like mouse ,printer etc their info stored in this file. Essential device files. This includes terminal devices,USB or any device attach to the system.

### Shortcut Keys:

TAB:  Auto completes Name
Ctrl+ C : Cancel the Process Manually
Ctrl+ D : Same as above command
Ctrl +L : Clear the screen
Ctrl + alt + D : Minimize all terminals/windows
Ctrl + U : Clear the line
Ctrl + Z: Suspend Process for background (fg for revert)
Ctrl + A: for starting point
Ctrl + E: for Ending point

#### How to Update your System:
./    (Executes the shell file)
bash (Executes Shell Programs)


### Inode
An Inode (index node) is a data structure used by Linux file systems to organize file content on disk. It is a key component of the Unix file system architecture and is used to maintain the file system's metadata, such as the file name, file permissions, file size, and dates. Each file is represented by a unique Inode number, and the Inode contains pointers to the location of the actual file data on disk. Inodes are often used by file system tools and utilities to manage file access and retrieval.