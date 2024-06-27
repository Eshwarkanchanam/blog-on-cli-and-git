# CLI - Some commonly used commands

## What is CLI (Command Line Interface)?

 - A command line interface (CLI) is a software mechanism you use to interact with your operating system using your keyboard.
 - In the early days of computing, instructions were provided using binary language, which is difficult for all of us to read and write.Therefore, in an operating system, there is a special program called the shell. The shell accepts human-readable commands and translates them into something the kernel can read and process.

## Some Commonly used commands

### Basic Linux Commands to Run in the Terminal
` whoami ` - This command prints the name of the currently logged in user to the terminal session.
```
caesarsage@caesarsage:$ whoami
```

` man ` - This command prints the manual or information about a command, configuration files, and so on. This command is very useful when it comes to getting more information about any command.
```
caesarsage@caesarsage:$ man whoami
```

` clear ` - Clears all previous commands that were run in the current terminal. This clears the screen from previous commands in the terminal.
```
caesarsage@caesarsage:$ clear
```

## How to Work with Directories in Linux

` pwd ` - It should print the current folder/directory path where you currently are.
```
$:~/Documents/github.com$ pwd
```

` cd <path> ` - You can change your current directory with the cd command (Change Directory). Just like going back and forth between folders when using the GUI.
```
$: cd Documents/articles
```

` cd ~ ` - The cd is also a shortcut to get back into your home directory. Just typing cd without a target directory will put you in your home directory. Typing cd ~ has the same effect.
```
$:~/Documents/github.com$ cd ~
```

` cd .. ` - To go to the parent directory (the one just above your current directory in the directory tree), type cd ..:
```
$:~/Documents/github.com$ cd ..
```


` ls ` - Inside a folder you can list all the files that the folder contains using the ls command. It takes no arguments.
```
$:~/Documents/mycatfolder$ ls
```

` mkdir <directoryName> ` - will create directories
```
$:~/Documents$ mkdir cats
```

` rmdir <directoryName> ` - When a directory is empty, you can use rmdir to remove or delete the directory.
```
$ rmdir cats
```

` touch ` - used to generate empty files.
```
$ touch <filename>...
# alternatively you can also create empty file by using
$ cat > <filename>
# or
$ > <filename>
```

### Commands for pattern searching 

` grep ` - used to globally search for regular experssion and printing matching lines

syntax : ` grep [options] pattern [files] `

   | option | description |
   | :-----: | :-----------|
   |-i      | search for a string case insensitively |
   |-c      | count of no of lines matches given string |
   |-w      | by default grep matches string/pattern even if it is found as a substring in file.with -w option it matches the whole word |
   |-o      | display only matched pattern | 
   |-n      | show line number while displaying output |
   |-v      | inverting the pattern matches |
         
```
$ grep -i linux linux.txt
# above command will search for linux word in linux.txt file case insensitively
```

` find ` - used to find file and directories searches within hierarichal structure.

  - can do search by name , modification time , size.

syntax : ` find [path] [options] [expression] `

| option | description |
| :-----:| :-----------|
| -name | search with a specific file name or pattern |
| -iname | case insensitive version of -name option |
| -perm | search with specific permission of a file |
|-type | specific type of file or directory (f for regular files) ( d for directories ) |
| -size [+/-]n | +n for larger files -n for smaller files |
| -empty | find empty files or directories |
| -delete | deletes files that matches specific criteria |
| -exec comm {} \; | execute a command on each file and directory found |

```
$ find ~/ -type f -name '*.log'
# above command will search for files in user directory type will be file and names matchinf with .log extension 
```

### Difference between grep and find 
- the only difference between find and grep is that grep used to search for pattern inside a file where as find is used to search in file or directory names

## Some useful resources

- cli cheatsheet [https://www.git-tower.com/blog/command-line-cheat-sheet/](https://www.git-tower.com/blog/command-line-cheat-sheet/)
- cli documentaion [https://docs.rockylinux.org/books/admin_guide/03-commands/](https://docs.rockylinux.org/books/admin_guide/03-commands/)
- cli video tutorial [https://www.youtube.com/watch?v=uwAqEzhyjtw&t=120s](https://www.youtube.com/watch?v=uwAqEzhyjtw&t=120s)

