1. Creating files and directories
Command	Purpose
touch file1.txt	Creates an empty file
echo "Hello, Linux" > file2.txt	Creates a file and writes text into it
mkdir testdir	Creates a directory (folder)
echo "Hidden file" > .hiddenfile	Creates a hidden file

touch creates an empty file if it doesn't exist. If the file already exists, it updates its timestamp without replacing its content.
echo displays text, but when combined with >, it redirects that text into a file.
> overwrites existing file content if the file already exists.
Linux files beginning with a dot (.) are hidden by convention.
 mkdir means make directory.

2. Listing files and directories
ls	Lists files and directories
ls -l	Shows a detailed listing
ls -a	Shows hidden files too
ls -la	Shows hidden files in detailed format
ls -l testdir	Lists the contents of a specific directory
ls -R tem p_dir	Listscontents recursively, including subdirectories

The ls command allows us to view the contents of directories.
 -l displays details such as permissions, ownership, size and modification time.
 -a includes hidden files.
 -R lists contents recursively.

3. Copying files and directories
Command	Purpose
cp file1.txt file1_copy.txt	Copies a file
cp file2.txt testdir/	Copies a file into a directory
cp -r testdir testdir_copy	Copies a directory and its contents

cp means copy.
Copying a file creates another file without removing the original.
-r means recursive and is needed when copying directories and their contents.

4. Moving and renaming files and directories
The mv command is used to move files or directories and to rename them.
Command	Purpose
mv file1.txt newname.txt	Renames a file
mv newname.txt testdir/	Moves a file into a directory
mv testdir_copy new_testdir	Renames a directory
mv testdir/newname.txt ./original_file1.txt	Moves and renames a file


 mv means move.
 The same command can be used to rename files and directories.
./ refers to the current directory.

5. Removing files and directories
Linux deletion commands require care. Deletion through the terminal may not go to a recycle bin.
Command	Purpose
rm original_file1.txt	Removes a file
rm -i file2.txt	Prompts before removing a file
rmdir new_testdir	Removes an empty directory
rm -r testdir	Removes a directory and its contents recursively
rm .hiddenfile	Removes a hidden file
mkdir temp_dir	Creates a temporary directory
touch temp_dir/temp_file.txt	Creates a file inside the directory
ls -R temp_dir	Lists the directory recursively
rm -rf temp_dir	Forcefully removes a directory and its contents

 rm means remove.
-i means interactive and asks for confirmation.
rmdir removes empty directories only.
 rm -r removes a directory and its contents recursively.
-f means force and suppresses prompts and certain errors.
rm -rf is powerful and dangerous because it removes directory contents without interactive confirmation.
