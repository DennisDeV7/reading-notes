# Bash Command Line Tutorials

## The Command Line

The command line, or terminal, is a text based interface to the computer. The way to open a terminal is different depending on the operating system but here are some basic ways for mac and linux. For mac, go to Applications -> Utilities and find Terminal. For linux (Ubuntu) you can go to Applications -> System or my favorite is to just use ctrl+alt+t.

The shell is a part of the operating system that defines how the terminal will behave after running commands. The most common is the bash shell, although for class we downloaded zsh. A useful shortcut is to press the uparrow to access a previously executed command.

----

## Basic Navigation

The shell offers different command that can help navigate through it to help find files, see the contents of the files, and change the directory. See below for a short list of navigation commands:

- pwd: Print Working Directory - shows the path of the current directory
- ls: lists the contents of the directory
- ls -l: lists the contents of the directory in a long list with more details about the files
- ls -a: lists all of the contents including hidden files
- cd: Change Directory - moves the user to a different directory\

Shortcuts:

- ~ : Shortcut to the home directory
- . : refers to the current directory
- .. : refers to the parent directory, you can use this several times to keep going up in the directory

----

## More About Files

Everything on a linux system exists in the form of a file. In addition, Linux is an extensionless system, it determines the type of file by reading the contents not by a file extension. Some other things to take note when using a linux system is: it is case sensitive, it does not see spaces in names, and you can use escape characters in the command line to alter the behanvior such as (\). Within most computers are hidden files.  These are files that are marked to be hidden so they do not interfere with the user. Using ls -a you can view these hidden files so that you can open them or just view them. On linux a hidden file simply has a "." on the beginning of the filename.

----

## Manual Pages

Manual Pages are an option that shows an explaination of the given command. These are helpful so you do not have to remember all of the commands you only have to remember how to look it up. For example:

man `<command to look up>`

You can also do a key word search if you do not know what command  to enter by using the following:

man -k `<search term>`

----

## File Manipulation

Linux comes with convenient commands to manage a file directory. This is extremely important for organizing a project so you do not have to search through a folder with hundreds of files. To create a directory you can use the following command: 

mkdir `[options]<Directory>`

Some common supporting commands may include  -p or -v

- -p: tells the command to make parent directories as needed
- -v: will display all of the actions that mkdir is performing in the background

Below are a list of other useful commands for file manipulation

- rmdir `[options]<Directory>`: Removes a directory
- touch `[options]<filename>`: Creates a blank file
- cp `[options]<source><destination>`: copies the source file to the destination folder
When we use cp the destination can be a path to either a file or directory. If it is to a file (such as examples 1, 3 and 4 above) then it will create a copy of the source but name the copy the filename specified in destination. If we provide a directory as the destination then it will copy the file into that directory and the copy will have the same name as the source. - ryanstutorials.net

- mv `[options]<source><destination>`: behaves similarly to cp except it just moves the file.
- rm `[options]<file>`: removes a file

----

## Cheat Sheet

Below is a link to a cheat sheet to help as a quick reference to any of the above material

[Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)