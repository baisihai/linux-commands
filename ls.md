## ls Command
List files and directories.

## Syntax
```bash
ls [option] [file/directory]

Options	Description
-l	known as a long format that displays detailed information about files and directories.
-a	Represent all files Include hidden files and directories in the listing.
-t	Sort files and directories by their last modification time, displaying the most recently modified ones first.
-r	known as reverse order which is used to reverse the default order of listing.
-S	Sort files and directories by their sizes, listing the largest ones first.
-R	List files and directories recursively, including subdirectories.
-i	known as inode which displays the index number (inode) of each file and directory.
-g	known as group which displays the group ownership of files and directories instead of the owner.
-h	Print file sizes in human-readable format (e.g., 1K, 234M, 2G).
-d	List directories themselves, rather than their contents.
```

## Examples
1. List files and directories.
```bash
ls
```

2. Display all information about files/directories.
```bash
ls -l
```

3. List files and directories, including all the hidden files in the directory.
```bash
ls -a
```

4. Display file sizes in a human-readable format.

```bash
ls -lh
```

5. Order files based on last modified time.

```bash
ls -lt
```

6. Order files based on last modified time (in reverse order).

```bash
ls -ltr 
```

7. List files and directories in /etc directory.

```bash
ls /etc
```
