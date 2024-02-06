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