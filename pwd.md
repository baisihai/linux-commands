## pwd Command
Print current working directory.

## Syntax
```bash
pwd [OPTIONS]
```
Options	Description
-L	resolves symbolic links and prints the path of the target directory. The default behavior of the shell built-in “pwd” is equivalent to using “pwd -L”.
-P	displays the actual path without resolving symbolic links. The default behavior of the binary “/bin/pwd” is the same as using “pwd -P”

## Examples
1. Display the current directory using built-in pwd (pwd). The default behavior of Built-in pwd is the same as pwd -L. If current directory is a symbolic link, then it returns the symbolic path of the current directory. 
```bash
pwd
```

2. Display the current directory using Binary pwd (/bin/pwd). The default behavior of /bin/pwd is the same as pwd -P. It displays the actual path, ignoring symbolic links.
```bash
/bin/pwd
```

3. The $PWD environment variable. The $PWD environment variable is a dynamic variable that stores the path of the current directory. It holds the same value as ‘pwd -L’ (if necessary, it returns the symbolic path).
```bash
echo $PWD
```
