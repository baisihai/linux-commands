## rmdir Command
Remove empty directories.

## Syntax
```bash
rmdir [option]... [directory]...

Options                     Description
--ignore-fail-on-non-empty  It prevents the errors if the directory is not empty.
-p or --parents	            It will removes the directory and its parent directories if they are empty.
-v or --verbose	            It helps in displaying the message for each directory that is removed.
--help	                    It will displays the helpful information and exits.
--version	                It displays version information and exits.
```

The rmdir command won’t work if the directory contains subfolders. To force the deletion, add the –p option. Note that you must own the item you want to remove or use sudo instead.

## Examples
1. Deletes the empty directory named "temp".
```bash
rmdir temp
```

2.  Removing more than one directory at a time.
```bash
rmdir temp1 temp2 temp3
```

3. Delete a directory, including all the subdirectories.
```bash
rmdir -p temp1/temp2/temp3/...../tempN
```

4. Display the message after removing each directory.
```bash
rmdir -v temp1 temp2 temp3
```

5. Remove multiple directories with the same expression
```bash
ls 
temp1
temp2
temp3

rmdir -v temp*
rmdir: removing directory, 'temp1'
rmdir: removing directory, 'temp2'
rmdir: removing directory, 'temp3'
```

6. Ignore the errors due to the non-empty directories.

Sometimes we get the following error while removing a directory through the rmdir command:
```bash
rmdir temp
rmdir: failed to remove 'temp': Directory not empty
```
We can use the –ignore-fail-on-non-empty to ignore the errors due to the non-empty directories. For instance, let’s remove the temp directory that contains sub-directories:
```bash
rmdir temp 
rmdir  --ignore-fail-on-non-empty temp
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
