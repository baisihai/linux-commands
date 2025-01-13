## rm Command
Remove files and directories.

## Syntax
```bash
rm [options] file1 file2...

Options  Description
-r       Remove directories recursively.
         By default, rm command does not remove directories. 
-f       Force removal without confirmation.
-i       (Interactive Deletion): The -i option makes the command ask the user for confirmation before removing each file.
         You have to press y to confirm deletion, any other key leaves the file un-deleted.
```

## Examples
1. Deletes the file named "test.txt".
```bash
rm test.txt
```

2.  Removing more than one file at a time
```bash
rm test1.txt test2.txt test3.txt
```

3. Deletes the directory “my_directory” and its contents.
```bash
rm -r my_directory
```

4. Forcefully deletes the file "test.txt" without confirmation.
```bash
rm -f test.txt
```

5. Deletes the file "test.txt" with user confirmation.
```bash
rm -i test.txt
```

## Difference between ‘rmdir’ and ‘rm’ Command
The following are the differences between rmdir and rm command:

| Aspect	| rmdir Command	| rm Command	|
|-------------|------|--------|
| Primary Function	| Removes the empty directories	| Remove files and directories	|
| Usage Limitation	| Can only remove empty directories	| Can remove both empty and non-empty entities	|
| Recursive Deletion	| Not applicable 	| Can delete directories and their contents recursively with -r option	|
| Safety	| Safer. It only deletes if directories are empty	| Requires caution, especially with -r and -f options	|
| Command Complexity	| Simple and straightforward	| More complex with multiple options and flags for different use cases	|
