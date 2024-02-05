# LINUX COMMAND AND BASIC IMPLEMENTATION

## HOW TO CREATE FILE IN LINUX

### 1.cat command

#### 1.1 cat command is used to create files.
<br>

#### STEPS

$ cat > file1
<br>
then ctrl+d
<br>
$ ls (Created files will be shown)
<br>
$ cat file1 (to see the content)
<br>

#### 1.2 cat command is not editor once file is created its content cannot be edited but new content can be added.

#### STEPS

$ cat >> file1
<br>
$ cat ls
<br>

#### 1.3 cat command is used to concatenate files
<br>

#### STEPS

cat file1 file2 > file3
(Concatenation happens and new file3 will have all content )


<br>


#### 1.4 cat command is used to copy files 

<br>

#### 1.5 cat command is used to read from bottom to first
<br>

#### STEPS
<br>

tac file1


### 2.touch command (For changing timestamp)
<br>

![touch command](allimage/image14.png)

### 3.vi/vim command(IT IS EDITOR ALSO)
<br>

![vi command](allimage/image15.png)

#### STEPS FOR USING vi/vim commands

<br>
vim file1
<br>
press i in keyboard
<br>
add text or edit text
<br>
press esc
<br>
then press :wq
<br>

### 4.nano command
<br>

#### STEPS

nano file2
<br>
write or edit
<br>
ctrl x
<br>
shift+y
<br>
enter
<br>