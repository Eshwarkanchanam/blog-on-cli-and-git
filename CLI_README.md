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
casesarsage@caesarsage:~/Documents/github.com$ pwd
```
` cd <path> ` - You can change your current directory with the cd command (Change Directory). Just like going back and forth between folders when using the GUI.
```
caesarsage@caesarsage$: cd Documents/articles
```
` cd ~ ` - The cd is also a shortcut to get back into your home directory. Just typing cd without a target directory will put you in your home directory. Typing cd ~ has the same effect.
```
caesarsage@caesarsage:~/Documents/github.com$ cd ~
```
` cd .. ` - To go to the parent directory (the one just above your current directory in the directory tree), type cd ..:
```
caesarsage@caesarsage:~/Documents/github.com$ cd ..
```


` ls ` - Inside a folder you can list all the files that the folder contains using the ls command. It takes no arguments.
```
caesarsage@caesarsage:~/Documents/mycatfolder$ ls
```
` mkdir <directoryName> ` - will create directories
```
caesarsage@caesarsage:~/Documents$ mkdir cats
```
` rmdir <directoryName> ` - When a directory is empty, you can use rmdir to remove or delete the directory.
```
caesarsage@caesarsage~/Documents$ rmdir cats
```

