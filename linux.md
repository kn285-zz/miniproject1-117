# **Vim and Linux**

## *Vim Editor*

-------------------------

### Insert Mode

The shortcut is: "i"
The Insert mode lets you insert text in a document.  (insert text where the cursor is) or "o" (insert text at the beginning of the following line).

### Visual Mode

The shortcut is: "V"
The visual mode permits the user to select the text as you would do with a mouse but using the keyboard instead of the mouse. Useful to copy several lines f text for example.

### Command Mode

Command begins with the symbol ":"
When you are in another mod you can use the escape key (sometimes you'll need to hit it twice) to come back to command mod at any time.

------------------

### Vim Usage Example

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

### Vim Command Referenece

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

## *Basic Linux Commands*  
-------------------------------  

### Home Directory
Home Directory is the default directory that a user places into when the user logs in. The username is typically where the files are listed under
```
/                    # The root of the filesystem
└── home             # A directory named home
    └── vagrant      # A directory named vagrant
        └── myfile   # A file named myfile
```

### Tildo

Character: ~  
The Tildo is a character used that refers to the current user's home directory.

### CD

The "CD" command stands for "change directory." As the name suggests it used to change the directory. If the commands has no argument then it take you to   the home directory.

### mkdir

"mkdir" command in Linux allows the user to create directories (also referred to as folders in some operating systems ). This command can create multiple directories at once as well as set the permissions for the directories.
```
$ mkdir [options...] [directories ...]
$ mkdir NewDirectory
```
### Copying Files (cp)
cp refers to copy. You can make a copy of a file or directory using cp command. -r use it for folders to copy internal recursive files, otherwise folder copy will not work.
```
$ cp welcome.txt welcome_copy.txt
```
### Print Working Directory (PWD)
It refers to print working directory. It prints the absolute path of directory where you are in right now.
```
$ pwd
/home/root
```
### mv
The "mv" command is used to move files. You can use absolute or relative paths when moving files. You can also change the name of the destination file.  

This command is used to move a file.
```
$ mv /home/vagrant/file01 /tmp/file01
```
This command is used to move and change the name of the file  
```
$ cp /home/vagrant/file01 /tmp/newfile
```
### rm

The "rm" command is used to delete files and directories.  
Use this command to delete a file:
```
$ rm /tmp/file01
```
Use this command to recursively remove all files in a directory:
```
$ rm -r /tmp/dir01
```
Use this command to skip the confirmation prompt for removing a file:
```
$ rm -f /tmp/file01
```
### history
"history" is a command that shows the last 500 commands you've entered.
```
$ history
```
You can use "-c" to clear the history buffer
```
$ history -c
```
You can use "!!" to rerun the previous command
```
$ !!
```
You can also use ""!N" where "N" is the number of the command from the history command output.
```
$ !5
```
