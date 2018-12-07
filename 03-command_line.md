# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

`pwd` - print working directory
`ls` - list all files and directories in the current working directory
`cd` - change directory ('..' brings you to the parent directory, '/' to the root directory)
`mkdir` - makes a directory
`touch` - creates a new file inside the working directory
`rm` - remove a file or directory
`clear` - clear screen

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  
  
> `ls`  - lists all files and directories in the current working directory  
> `-a`  - lists all files and directories including hidden files  
> `-l`  - lists long format (includes permissions) with file size  
> `-lh`  - lists long format with readable file size  
> `-lah`  - lists long format including hidden files with readable file size  
> `-t`  - lists sorted by time & date  
> `-Glp`  - excludes owner name, lists long format, and adds a '/' at the end of all directories  

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> `-r` - lists in reverse order  
> `-R` - includes sub-directories  
> `-d` - only lists directories  
> `~` - lists home directory  
> `-1` - displays each entry on its own line  

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> `xargs` allows us to build an execution pipeline with standard inputs.  
> An example would be to use `echo 'a.txt b.txt c.txt' | xargs touch`  
> This would look like:  
> ```
> echo 'a.txt b.txt c.txt' | xargs touch
> ls
> a.txt b.txt c.txt
```

 

