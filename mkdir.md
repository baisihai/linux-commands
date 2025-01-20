## mkdir Command
Create a new directory.

## Syntax
```bash
mkdir [options...] [directory_name]

Options          Description
–help            Displays help-related information for the mkdir command and exits. Use this option to get assistance on how
                 to use the command and its various features.
–version         Displays the version number and additional information about the license for mkdir, providing details about
                 the software version installed. Use this option to check the installed mkdir version.
-v or –verbose   Enables verbose mode, displaying a message for every directory created. When used with the [directories]
                 argument, it shows the names of the directories being created.
-p               A flag that allows the creation of parent directories as necessary. If the specified directories already
                 exist, no error is reported. Useful for creating a directory hierarchy without errors.
-m               Sets file modes or permissions for the created directories. The syntax follows that of the chmod command.
                 Use this option to specify permissions, such as read, write, and execute, for the new directories.
```

## Examples
**1. Create a new directory named "test".**
```bash
mkdir test
```

**2. Display a message for every directory created. In this example, 3 directories named "test1", "test2" and "test3" are created.**
```bash
mkdir -v test1 test2 test3
```

**3.  Create a new directory named "third", and to create parent directories as necessary. In this example, directories "first" and "second" are created if they do not exist.**
```bash
mkdir -p first/second/third
```

**4.  Create a new directory named "test", and set the file modes (i.e. permissions).**
```bash
mkdir -m a=rwx test
```
