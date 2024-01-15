## CSE 15L Lab Report 1


### `cd`
1. using the command with no arguments
	
	command: `cd`
	
	output: ` ` 
	
	`pwd`: `/home`
	
	I got a blank output because the command `cd` is "change directory" and it directs you to a specific directory that you want to work on. However, not providing a specific directory after `cd`, the computer does not know which directory you want to use, therefore it cannot perform any action and is not an error.
2. using the command with a path to directory as argument

	command: `cd lecture1`
	output: `[user@sahara ~]$` changed to `[user@sahara ~lecture1]$`
	
	`pwd`: `/home/lecture1`
	
	"Lecture1" appears after user, which means that the working directory changed from home to lecture1. This is not an error because `cd` means change directory, and by providing a specific directory after `cd` it takes you to exactly that directory.
3. using the command with a path to file as argument

	command: `cd Hello.java`
	
	output: `bash: cd: Hello.java: Not a directory`
	
	`pwd`: `/home/lecture1`
	
	The output tells you that `Hello.java` is not a directory. This is an error because `cd` is designed to put you in a directory instead of a specific file.


## `ls`

1. using the command with no arguments

	command: `ls`
	
	output: `Hello.class Hello.java messages README`
	
	`pwd`: `/home/lecture1`
	
	I got this output because `ls` lists all the files in the current directory, and it did list all the files. This is not an error because it printed what was needed.
2. using the command with a path to directory as argument
	
	command: `ls messages`
	
	output: `en-us.txt es-mx.txt zh-cn.txt`
	
	`pwd`: `/home/lecture1`
	
	I got this output because `ls` should list all the files in the `messages` directory and it did, so there is not an error.
3. using the command with a path to file as argument

	command: `ls Hello.java`
	
	output: 	`Hello.java`
	
	`pwd`: `/home/lecture1`
	
	The output restates the file name that I wrote in the command. When `ls` is used on a file, that specific file is what it identifies. There is not an error.


## `cat`
1. using the command with no arguments

	command: `cat`
	
	output:
	
	`pwd`: /home
	
	The output is blank, which makes sense since there is no content from a file to display. However, I foundthat once I type `cat`, anything I input from then on will be repeated at the terminal. There is not an error.
	
2. using the command with a path to directory as argument

	command: `cat lecture1`
	
	output: `cat: lecture1: Is a directory`
	
	`pwd`: `/home`
	
	The output says that `lecture1` is a directory and did not print any specific content from files, which means concatenating a directory will not automatically display the content of its files. You have to provide specific file names. There is no error.
	
	
3. using the command with a path to file as argument

	command: `cat en-us.txt`
	
	output: `Hello World!`
	
	`pwd`: `/home/lecture1/messages`
	
	The output prints the content of en-us.txt okay. However, because I was in the home directory at first, the computer couldn't find en-us.txt, so I had to use `cd` and went into the messages directory first to `cat` the file. There is no error.
