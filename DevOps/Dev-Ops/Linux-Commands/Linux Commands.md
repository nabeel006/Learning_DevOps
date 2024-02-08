

Record Your Activity in Terminal with Output:

Helpful while doing Task.

|   |
|---|
|script (create TypeScript Name File)  <br>Ctrl + d (exit from script)|

  
  
  

Check Current Location:

Current Logged-in User 

Check Date And Time

  

|   |
|---|
|timestamp=$(date "+%Y-%m-%d %H:%M:%S")  <br>nabeel@Nabeel:~$ echo "$timestamp"  <br>2024-01-29 10:14:35  <br>nabeel@Nabeel:~$ timestamp=$(date "+%H:%M")  <br>nabeel@Nabeel:~$ echo "$timestamp"  <br>10:16  <br>nabeel@Nabeel:~$ timestamp=$(date "+%M")  <br>nabeel@Nabeel:~$ echo "$timestamp"  <br>16|

  
  

|   |
|---|
|pwd  <br>  date  <br>  whoami  <br>  date +%D  <br>  date +%T  <br>  date +%H:%M|

  
  
  
  

How to display Files and list in the current directory

|   |
|---|
|1135  ls  <br>1136  ls -lt    /display the expanded list of folders  <br>1137  ls -la    //display hidden file also  <br>1138  ls -ltr   //shows in reverse order and latest will be in the end  <br>1139  ls -lh    //human readable form|

  

|   |
|---|
|Terminal clean:  <br>Ctrl+L  //   clear|

  
  
  

Display Content on Terminal:

Cat command

  

How to read a file and search for a word:

  

|   |
|---|
|less command for reading the file and search for a text into there  <br>  <br>/(word)  top to bottom search  <br>Ctrl+ g  bottom to top  <br>  <br>N for next|

  

See the Page by Page Content:

More —-----------ENter (line by line)

Below arrow for page by page

  
  

How to Create File:

Touch filename

How to delete:

Rm filename 

  

Edit:

 vi  newfile and enter

(i insert)

(shift + :  Save)

wq(write and quite

  

|   |
|---|
|nano (directly write|

  
  

Make Directory:

  

|   |
|---|
|mkdir newFolder|

  
  

|   |
|---|
|rmdir foldername)|

  

 Remove Dir  rm -rf name

  

Relative  and Absolute Path:

  

Exact path  starting from the root directory is Absolute Path

  

Give the path with relation of current directory to go in the relative path.

  
  

|   |
|---|
|nabeel@Nabeel-DevOps:/opt/lampp/htdocs$ cd /opt/lampp/htdocs  <br> <br><br>nabeel@Nabeel-DevOps:/opt/lampp/htdocs$ cd crud-proj|

  
  
  

|   |
|---|
|cp  <br>mv  <br>sort  <br>uniq|

  

Wild Cards: *  ,   [ ]   , {1..10}

  

|   |
|---|
|ls p*  <br>ls *.md  <br>touch file{1..10}  <br>rm file{1..10}|

  
  

Shuffle a file

|   |
|---|
|shuf filname|

CountNo of Lines and words and bytes in file

  

wc file  
wc -l file

  

How to check the file are identical or not:

  

Cmp command

  

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop/dir1$ cat >>fil2  <br>Hello  <br>My Name is Nabeel  <br>Thanks  <br>^C  <br>nabeel@Nabeel-DevOps:~/Desktop/dir1$ cat >>fil3  <br>Hi  <br>My Name is Qamar  <br>Thank You  <br>^C  <br>nabeel@Nabeel-DevOps:~/Desktop/dir1$ cmp fil2 fil3  <br>fil2 fil3 differ: byte 2, line 1|

  

Diff Command

  

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop/dir1$ diff fil2 fil3  <br>1,3c1,3  <br>< Hello  <br>< My Name is Nabeel  <br>< Thanks  <br>---  <br>> Hi  <br>> My Name is Qamar  <br>> Thank You  <br>nabeel@Nabeel-DevOps:~/Desktop/dir1$ diff -u fil2 fil3  <br>--- fil2 2024-01-25 11:35:55.808306306 +0500  <br>+++ fil3 2024-01-25 11:36:24.268439550 +0500  <br>@@ -1,3 +1,3 @@  <br>-Hello  <br>-My Name is Nabeel  <br>-Thanks  <br>+Hi  <br>+My Name is Qamar  <br>+Thank You|

  

How to Find File in Linux:

|   |
|---|
|nabeel@Nabeel-DevOps:~$ locate fil1  <br>/home/nabeel/Desktop/dir1/fil1  <br>/home/nabeel/Desktop/dir1/fil10  <br>nabeel@Nabeel-DevOps:~$ find ./ -name fil3  <br>./Desktop/dir1/fil3  <br>nabeel@Nabeel-DevOps:~$|

  
  

Using Locate : 

It is most usefulthan find it has its own db like cache but it has one problem that is it needs to update the Db so we update the DB then it will also find the new file.

|   |
|---|
|nabeel@Nabeel-DevOps:~$ touch Desktop/dir1/nabeel.txt  <br>nabeel@Nabeel-DevOps:~$ find ./ -name nabeel.txt  <br>./nabeel.txt  <br>./Desktop/dir1/nabeel.txt  <br>nabeel@Nabeel-DevOps:~$ locate nabeel.txt  <br>nabeel@Nabeel-DevOps:~$ sudo updatedb  <br>nabeel@Nabeel-DevOps:~$ locate nabeel.txt  <br>/home/nabeel/nabeel.txt  <br>/home/nabeel/Desktop/dir1/nabeel.txt|

  
  

History:

|   |
|---|
|nabeel@Nabeel-DevOps:~$ history \| grep sort  <br>1171  sort fil.txt  <br>1172  sort fil.txt \| uniq  <br>1245  history \| grep sort|

Help command:

Man command

  

Calculator in Linux: and Calendar in Linux

|   |
|---|
|bc<br><br>sudo apt install ncal -y<br><br>cal<br><br>cal August 2024<br><br>cal August|

How to check how long your server is running

How much user is logged in in the current session

  

|   |
|---|
|nabeel@Nabeel-DevOps:~$ uptime  <br>12:30:16 up  2:45,  1 user,  load average: 3.49, 2.90, 2.54 (System Resource Utility)|

  

How to make shortcut in Alias:

Helpful to cover the long commands

  

alias -p

  
  
  

# How to Zip or comprress a File and Keep the original as well:

  

Its just compress the files only

  

|   |
|---|
|nabeel@Nabeel-DevOps:~$ gzip -k nabeel.txt  <br>nabeel@Nabeel-DevOps:~$ rm nabeel.txt  <br>nabeel@Nabeel-DevOps:~$ ls  <br>crudapp    google-chrome-stable_current_amd64.deb  Pictures   travellist  <br>Desktop    javasharedresources                     Public     typescript  <br>Documents  Music                                   snap       Videos  <br>Downloads  nabeel.txt.gz                           Templates  <br>nabeel@Nabeel-DevOps:~$ gunzip nabeel.txt.gz  <br>nabeel@Nabeel-DevOps:~$ ls  <br>crudapp    google-chrome-stable_current_amd64.deb  Pictures   travellist  <br>Desktop    javasharedresources                     Public     typescript  <br>Documents  Music                                   snap       Videos  <br>Downloads  nabeel.txt                              Templates|

  
  
  

In summary, tar is primarily for creating archives, gzip is for compressing individual files, and zip is for creating compressed archives with support for multiple files and directories. 

  
  

How to use ZIp Command:

And how to see only file in the zip without extract

  

|   |
|---|
|nabeel@Nabeel-DevOps:~$ cd newfolder  <br>nabeel@Nabeel-DevOps:~/newfolder$ touch fil1 fil2  <br>nabeel@Nabeel-DevOps:~/newfolder$ zip zipFil.zip fil1 fil2  <br>  adding: fil1 (stored 0%)  <br>  adding: fil2 (stored 0%)  <br>nabeel@Nabeel-DevOps:~/newfolder$ ls  <br>fil1  fil2  zipFil.zip  <br>nabeel@Nabeel-DevOps:~/newfolder$ unzip zipFil.zip  <br>Archive:  zipFil.zip  <br>replace fil1? [y]es, [n]o, [A]ll, [N]one, [r]ename: y  <br>extracting: fil1                     <br>replace fil2? [y]es, [n]o, [A]ll, [N]one, [r]ename: y  <br>extracting: fil2                     <br>nabeel@Nabeel-DevOps:~/newfolder$ ls  <br>fil1  fil2  zipFil.zip  <br>nabeel@Nabeel-DevOps:~/newfolder$ unzip -l zipFil.zip  <br>Archive:  zipFil.zip  <br>  Length      Date    Time    Name  <br>---------  ---------- -----   ----  <br>        0  2024-01-25 13:01   fil1  <br>        0  2024-01-25 13:01   fil2  <br>---------                     -------  <br>        0                     2 files|

  
  
  

How to Download File from  the internet:

  

#wget URL_o_the_file

#wget -O filename  URL_of_the_file

  
  

How to Call API:

  

|   |
|---|
|#curl http://numbersapi.com/random|

  
  

How to install application : 

  

apt  (ubuntu)

  

yum/dnf (RedHat)

  
  

|   |
|---|
|sudo apt install nginx|

  

How to check an application is install or Not:

  
  

rpm -qa | grep app

#dnf list installed

  
  

|   |
|---|
|dpkg - -list \| grep app|

  
  
  

How to list available packages to install on linux

  

|   |
|---|
|#apt search <packg_Nme>|

Run and stop a Serveice:

List all services on system

  

|   |
|---|
|systemctl status mysql  <br>systemctl list-units --type=service --all|

  
  

Enviroment Variables:

  

|   |
|---|
|nabeel@Nabeel-DevOps:~$ echo $HOSTNAME  <br>Nabeel-DevOps  <br>nabeel@Nabeel-DevOps:~$ echo $HOSTTYPE  <br>x86_64  <br>nabeel@Nabeel-DevOps:~$ env|

  
  

|   |
|---|
|nabeel@Nabeel-DevOps:/usr/lib/jvm$ export JAVA_HOME="/usr/lib/jvm/java-1.11.0-openjdk-amd64"  <br>nabeel@Nabeel-DevOps:/usr/lib/jvm$ printenv  <br>  <br>nabeel@Nabeel-DevOps:/usr/lib/jvm$ export PATH=$JAVA_HOME/bin:$PATH  <br>nabeel@Nabeel-DevOps:/usr/lib/jvm$ java -version|

  
  

How to aDD it Permanently in Bash file because theseare are directly:

  

#add env variable in the ./bashrc file

#source ~/.bashrc_profile

  
  

|   |
|---|
|#vi ./bashrc (add your Variables)  <br>#export var_NAme  <br>#source .bashrc|

  
  

Print Specific Column from a csv File?

Read Data from CSV file and particular columns:

  

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop/Coding$ awk -F , '{print $NF}' test.csv  <br>Occupation  <br>Engineer  <br>Scientist  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ awk -F , '{print $1,$3}' test.csv  <br>Name  Occupation  <br>John  Engineer  <br>Jane  Scientist|

  

Getting Starting Characters of all Line:

Using CUT Command

  

Helpful in slicing the data

  

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop/Coding$ cut -c1-2 test.csv  <br>Na  <br>Jo|

Ja

  
  

Display Specific Line from a File:

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop/Coding$ sed -n '5p' test.csv  <br>John, 25, Engineer|

  

Replace a specific Word in File:

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop/Coding$ sed 's/John/Ahmar/g' test.csv  <br>Name, Age, Occupation  <br>Ahmar, 25, Engineer  <br>Jane, 30, Scientist  <br>Ali, 45,Engineer|

  
  
  

Upper and Lower the content within the file:

  

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop/Coding$ cat fil.txt  <br>a  <br>b  <br>d  <br>c  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ tr 'A-Z' 'a-z' < fil.txt  <br>a  <br>b  <br>d  <br>c  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ tr [:upper:] [:lower:] <test.csv  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ tr [:upper:] [:lower:] < fil.txt  <br>a  <br>b  <br>d  <br>c  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ tr [:lower:] [:upper:] < fil.txt  <br>A  <br>B  <br>D  <br>C  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ tr -d 'aeiou' <fil.txt  <br>  <br>b  <br>d  <br>C<br><br>  <br><br>Replace specific Word  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ tr 'b' 'a' <fil.txt  <br>a  <br>a  <br>d  <br>c|

  
  
  
  
  
  

Access Remote Linux Server:

  
  

|   |
|---|
|#ssh username@hostname  <br>#scp file user@hostname:/tmp/|

  
  
  
  

## How to change Permission and Ownership Change and Group Change:

  

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop/Coding$ sudo chown root xaa.txt<br><br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ ls -l xaa.txt  <br>-rwxrwxrwx 1 root nabeel 104857600 Jan 25 16:31 xaa.txt  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ sudo chgrp root xaa.txt  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ ls -l xaa.txt  <br>-rwxrwxrwx 1 root root 104857600 Jan 25 16:31 xaa.txt|

  

# Memory Info:

Check Free RAM Space

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop/Coding$ free -h  <br>              total        used        free      shared  buff/cache   available  <br>Mem:            15Gi       3.0Gi       7.9Gi       559Mi       4.6Gi        11Gi  <br>Swap:          2.0Gi          0B       2.0Gi  <br>nabeel@Nabeel-DevOps:~/Desktop/Coding$ free -th  <br>              total        used        free      shared  buff/cache   available  <br>Mem:            15Gi       3.0Gi       7.9Gi       559Mi       4.6Gi        11Gi  <br>Swap:          2.0Gi          0B       2.0Gi  <br>Total:          17Gi       3.0Gi       9.9Gi|

  
  
  

ALso check the memory and CPU utilization : 

top 

  
  

Disk Utilization will be helpful to monitor your space and check which folder causing the disk full and taking much space.

|   |
|---|
|nabeel@Nabeel-DevOps:~/Desktop$ du -h  <br>48K ./Investment-Binnce  <br>15M ./Coding/images  <br>193M ./Coding  <br>16K ./dir1  <br>205M .|

  
  
  

Check the file System and Disk Space Allocated 

  

|   |
|---|
|nabeel@Nabeel-DevOps:~$ df -h  <br>Filesystem      Size  Used Avail Use% Mounted on  <br>tmpfs           1.6G  2.3M  1.6G   1% /run  <br>/dev/nvme0n1p2  468G   22G  423G   5% /  <br>tmpfs           7.8G   90M  7.7G   2% /dev/shm  <br>tmpfs           5.0M  4.0K  5.0M   1% /run/lock  <br>efivarfs        154K   50K  100K  34% /sys/firmware/efi/efivars  <br>/dev/nvme0n1p1  511M  6.1M  505M   2% /boot/efi  <br>tmpfs           1.6G  136K  1.6G   1% /run/user/1000|

  
  
  

# System Info:

Check Hostanme /Server Name

  

|   |
|---|
|hostname|

Check CPU Core Thread info 

  

|   |
|---|
|lscpu|

  

Type of Architectur

|   |
|---|
|arch|

See the Partion Space and storage Allocation of the Disk;

|   |
|---|
|lslbk|

  

See the OS Name 

  

|   |
|---|
|uname -a  <br>  <br>cat /etc/os-release|

  
  
  

# Process Managment:

  

Is used to track the which app or task running on the server and the track this process and perform actions

**