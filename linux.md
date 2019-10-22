# **Vim and Linux**

### *Vim Editor*

-------------------------

#### Insert Mode

The shortcut is: "i"
The Insert mode lets you insert text in a document.  (insert text where the cursor is) or "o" (insert text at the beginning of the following line).

#### Visual Mode

The shortcut is: "V"
The visual mode permits the user to select the text as you would do with a mouse but using the keyboard instead of the mouse. Useful to copy several lines f text for example.

#### Command Mode

Command begins with the symbol ":"
When you are in another mod you can use the escape key (sometimes you'll need to hit it twice) to come back to command mod at any time.

------------------

#### Vim Usage Example

Example, editing of the file /etc/hosts
```
vim /etc/hosts
```

The editor is now in command mode. To start editing the file content, enter:
```
:i[enter]
```

Now you can edit the file by navigating to the line that you want to change with the cursor keys and then start typing the text. When you are finished with editing, press the [esc] key to go back to the command mode.

To save the file and exit the editor, enter:
```
:x[return]
```
In case you want to quit vim without saving the file, enter:
```
:q![return]
```

#### Vim Command Referenece

**save:**:w  
**save and exit:** :wq  
**exit:** :q  
**force:** ! (example :w! :q!)  
**vertical split:** open a document and then type :vsplit /path-to-document/document and this will open   the specified document and split the screen so you can see both documents.  
**copy:** y  
**copy a line:** yy  
**paste:** p  
**cut:** d  
**cut a line:** dd  

### *Basic Linux Commands*  
-------------------------------  

#### Home Directory

#### Tildo

Character: ~  
The Tildo is a character used that refers to the current user's home directory.

#### CD

The "CD" command stands for "change directory." As the name suggests it used to change the directory. If the commands has no argument then it take you to   the home directory.

#### mkdir

"mkdir" command in Linux allows the user to create directories (also referred to as folders in some operating systems ). This command can create multiple directories at once as well as set the permissions for the directories.
###### *Syntax:*
```
$ mkdir [options...] [directories ...]
$ mkdir NewDirectory
```
#### Copying Files (cp)
cp refers to copy. You can make a copy of a file or directory using cp command. -r use it for folders to copy internal recursive files, otherwise folder copy will not work.
```
$ cp welcome.txt welcome_copy.txt
```
#### Print Working Directory (PWD)
It refers to print working directory. It prints the absolute path of directory where you are in right now.
```
$ pwd
/home/root
```
#### mv
The mv command is used to move files. You can use absolute or relative paths when moving files.  

Moving the file from one directory to another
```
$ mv /home/vagrant/file01 /tmp/file01
```
Moving the file AND changing the name.
```
$ cp /home/vagrant/file01 /tmp/newfile
```



#### rm

The rm command is used to delete files and directories.  

Use this to delete a file.
```
$ rm /tmp/file01
```

To recursively remove all files in a directory, use the -r option.
```
rm -r /tmp/dir01
```
To skip the confirmation prompt for removing a file, use the -f option.
```
 rm -f /tmp/file01
```

#### history

The history command shows the last 500 commands that you've entered. you can also run "history -c" to clear the history buffer. If you want to rerun the last command in your history you can use the "!!" command. To run any other command you can run "!N" where "N" is the number of the command from the history command output. The command history for a user is located inside a file named ".bash_history" within the user's home directory.

```
$ history
```
