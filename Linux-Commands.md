# Linux Commands

## File Commands

- ```touch </path/file-name.ext>``` To create a file at a particular location with given extension.
- ```echo <some_content> > </path/file-name.ext>``` To create a file with some content at a particular location with the given extension.
- ```grep <some-string> <file-name.ext>``` Finds the particular string or regex in the given file.
- ```code </path/folder>``` Opens a folder at the provided path in the VS code.
- ```code .``` Opens the current folder in the VS code.
- ```code <file-name>``` Opens the file in the VS code.
- ```mv </path1/file-name1.ext> <path2/file-name2.ext>``` Moves or renames the file1 to file2.
- ```cat <file-name>``` Prints file content.
- ```cat <file-name_or_text> <more_files_or_text> >> <file-name>``` Concatenates files or texts then put them into a new file or same file.
- ```rm <file-name>``` Removes a file.
- ```rm -i <file-name>``` Removes the file while taking permission for each file name provided. 

## Directory Commands

- ```mkdir </path/dir-name>``` Creates an empty directory at the specified path.
- ```rmdir </path/dir-name>``` Deletes an empty directory at the specified path.
- ```rm -rf </path/dir-name>``` Deletes a non-empty directory at the specified path. ```r``` stands for recursive and ```f``` stands for forced.
- ```rm -d </path/dir-name>``` Deletes an empty directory at the specified path.
- ```gio open <some-path>``` Opens the file browser with the specified path.
- ```gio open .``` Opens the file browser with the current working directory.

## Command Chaining

- Command after the operator ```&&``` waits till the command before the operator is executed successfully.
- ```||``` means execute the command after the operator only if the preceding command fails.
- ```|``` is used to send the output of the preceeding command into the later command as an argument.
- ```&``` after a command makes it run in the background and is used for parallel execution of commands.
- ```;``` makes it possible to run several commands in a single go and the execution of the command occurs sequentially, irrespective of the fact whether the preceeding command execution was successfull or failure.
- ```<``` redirects input, i.e., transfers the content of the file after the operator into the command or function before the operator.
- ```<<``` is used when the input of the command before the operator should be taken directly from the terminal instead a file.
- ```<<<``` is used when a single string is to be passed as an input parameter for the preceeding command.
- ```>``` is used when writing an output of a command to a file (if file does not exists, then it will be created. If file exists, the content will be overwritten).
- ```>>``` is used when writing an output of a command to a file (if file does not exists, then it will be created. if file exists, the content will be appended).
- ```2>``` is used when writing the standard error of the command into a file and overwrites the content of the file. 2 is a file descriptor referring to ```STDERR```. Other file descriptors are 0 for standard input and 1 for standard output.
- ```&>``` is used when writing standard output and standard error if a command into a file and overwrites the content of the file.