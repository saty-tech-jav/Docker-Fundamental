# LINUX COMMAND AND ITS USE CASE MOSTLY RELATED TO DIRECTORY

## HOW TO CREATE DIRECTORY

<br>

1.mkdir devops1 (directory/folder will be created)

<br>

2.cd devops1 (switch to directory devops1)

<br>

3.mkdir devops1/devops2 (if devops1 directory is created then directory inside devops1 will be created )

<br>

4.mkdir -p dir1/dir2/dir3 (directory inside directory will be created)

<br>

5.pwd (to know the current path) -pwd:print working directory

<br>

6.cd ../../..  (come out from directory)

<br>

7.cd . (current directory)

<br>

8.cd devops1/devops2/devops3  (Switch directly to directory devops3)

<br>

9.cp file1 dire2  (copy file from 1 directory to another)

<br>



## CREATE HIDDEN FILE OR DIRECTORY

1.touch .abc  (Hidden file will be created)

<br>

2.ls -a (to see all the files)

<br>

3.mkdir .a (hidden directory)

<br>

4.sudo su (change to root user)

<br>

5.ls -l (it will give all list of directory and files if first alphabet is d then it is directory and if - then it is file)

<br>

6.ls -al

<br>

## COPY A FILE, CUT A FILE ,RENAME A FILE COMMANDS WITH DIFFERENT SCENERIOS

### COPY A FILE OR DIRECTORY

<br>

1.cp command is used for copying files and directories

<br>

#### CONDITION 1:Want to copy file content from file which is present in child directory to file which is present in parent directory and user is in child directory

<br>

1.cp file2 ../file1

<br>

#### CONDITION 2:Want to copy file content from file which is present in child directory to file which is present in parent directory and user is in parent directory

<br>


1.cp dire2/file2 file1

<br>

#### CONDITION 3:Want to copy file content from file which is present in Parent directory to file which is present in child directory and user is in Parent directory

<br>

1.cp file1 dire2/file2

<br>

#### CONDITION 4:Want to copy file content from file which is present in Parent directory to file which is present in child directory and user is in child directory

<br>

1.cp ../file1 file2

<br>

### CUT PASTE FILE IN DIRECTORY

1.mv file1 dire2

<br>

2.mv file1 ../  (From child directory to parent directory)

<br>

### RENAME FILE

1.mv file1 file2 (Rename will happen)

<br>

### DELETE COMMANDS

1.rm -rf dire1

<br>

### PAGE CONTENT COMMAND

<br>

1.less file55 (Content in single page will be displayed)
   To exit press "q"

<br>

2.head file55 (initial 10 lines will be displayed)

<br>

3.tail file55 (last 10 lines will be displayed)

<br>

4.more file55

<br>

5.history

<br>


## YUM UPDATE

<br>

1.yum update -y

<br>

2.yum install tree -y

<br>

3.tree

<br>

4.yum install httpd -y

<br>

## grep command

<br>

1.The grep filter searches a file for a particular pattern of characters and displays all lines that contain that pattern. The pattern that is searched in the file is referred to as the regular expression (grep stands for global search for regular expression and printout). 

<br>


2.SYNTAX: 2.1.grep -i "UNix" geekfile.txt
          <br>
          2.2.grep girl file3
<br>


## SORT OF FILE

<br>

1.sort file1

<br>

2.hostname 

<br>

3.hostname -i

<br>

4.ifconfig

<br>

## SERVICES

<br>

1.service httpd status

<br>

2.service httpd start

<br>

3.yum update httpd -y

<br>

4.yum remove httpd -y

<br>

5.service httpd stop

<br>

6.chkconfig httpd on (if we want on starting the system automatically it starts)

<br>

7.yum list installed (if we want to see which packages are installed)

<br>


## WHICH COMMAND

<br>

1.which git (it will throw the result )

<br>

 result:/mingw64/bin/git

 <br>

## ECHO COMMAND

<br>

1. echo "hello"

<br>

2.echo "hello" file1 (file will also created having hello written)

<br>

3.echo > file1 (content of file will be deleted)

<br>

## whoami

<br>

1.whoami