## mv Command
Move/rename files and directories.

## Syntax
```bash
mv [options] [source_file_name(s)] [Destination_file_name]

Option              Detail
--backup[=vcm]	    Make a backup of each existing destination file, using the version control method vcm.
                    If vcm is omitted, --backup behaves the same as -b (backups are created, using the default version
                    control method). See backing up files for details.
-b                  Like --backup, but does not accept a backup method. Instead, the method specified by the
                    VERSION_CONTROL environment variable is used. Simple backups are created if the variable is not set.
                    See version control methods for details.
-f, --force         Always overwrite existing files without prompting. This can be useful if you need to overwrite multiple
                    files whose permissions are read-only; if you don't specify -f, you are prompted for every file.
-i, --interactive   Prompt before overwriting an existing file, regardless of the file's permissions.
-n, --no-clobber    Never overwrite any existing file.
```
> [!NOTE]
> If more than one of the above options is specified, then only the final option you specify takes effect.

```bash
--strip-trailing-slashes            Remove any trailing slashes from each source argument.
-S, --suffix=suffix                 Specify the file name suffix to be used for all backup files. The default is "~".
-t, --target-directory=destination  Move all sources into the directory destination.
-T, --no-target-directory           Treat destination as a normal file, not as a directory.
-u, --update                        Don't overwrite files if they're newer. A move only happens if the destination file
                                    is older than the source file, or the destination file does not already exist.
-v, --verbose                       Provide verbose output. Print the name of every file moved.
--help                              Display a help message, and exit.
--version                           Display version information, and exit.
```

## Examples
**1. Rename a file.**
```bash
mv Old_file_name New_file_name
```
<br/>
  
**2. Move a file.**
```bash
mv Src_file Dest_directory
```
<br/>

**3. Move multiple files.**
```bash
mv Src_file1 Src_file2 Src_file3 Dest_directory
```
<br/>

**4. Rename a directory.**  
```bash
mv Src_directory Dest_directory
```
<br/>
  
**5. Move a file with `-i` option for user confirmation.**  
The `-i` option makes the `mv` command ask for confirmation before overwriting an existing file. If the file doesn’t exist, it will simply rename or move it without prompting.
```bash
mv -i Src_file Dest_file
```
<br/>

**6. Move a file with `-f` option**  
`mv` usually prompts for confirmation to overwrite the destination file if a destination file is write-protected. The `-f` option overrides this behavior, and `mv` will overwrite the destination file forcefully and deletes the source file.
```bash
mv -f Src_file Dest_file
```
<br/>

**7. Move a file with `-n` (no-clobber) option**  
 With `-n` option, `mv` prevents an existing file from being overwritten.
```bash
mv -n Src_file Dest_file
```
<br/>

**8. Move a file with `-b` (backup) option**  
With this option, it is easier to take a backup of an existing file that will be overwritten as a result of the `mv` command. This will create a backup file with the tilde character (~) appended to it. 
```bash
mv -b Src_file Dest_file
```
<br/>

**9. Display the version of `mv`**  
```bash
mv --version
```
