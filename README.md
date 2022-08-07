# Linux Commands

## File Management 

### PWD

- This command get the full path of the current working directory
```
pwd
```

### cd

- This command navigate to the last directory you were working in

```
cd - 
```

- This command navigate to the current user's home directory 
```
cd ~
```

- This command go the parent directory of current directory 
```
cd .. 
```

### LS

- This command list the files and directories in the current directory in long(table) format 

```
ls -l
```

- This command list information about the directory dir-name instead of its contents 

```
ls -ld dir-name
```

- This command list all files including the hidden ones 

```
ls -a
```

- This command appends a symbol at the end of a line name to indicate its type

```
ls -F
```

- This command list the files sorted by last modified time with most recently modified files showing at the top
```
ls -lt
```

- This command list the file size in human readble fomat

```
ls -lh
```

- This command shows all subdirectories recursively

```
ls -lr
```

- This command will generate a tree representing of the file system starting from the current directory

```
tree
```

### cp

- This command will copy the file from 'source' to 'destination' -p stands for preservation. It preserves the original attributes of file while copying like file owner, timestamp, group, premission.

```
cp -p source destination
```

- This command will copy source directory to specified destination recursively

```
cp -R source_dir destination_dir 
```

- This command moves/renames the file1 to file2

```
mv file1 file2
```

- This command ask you before every file removal for confirmation. You can specify multiple files. 

```
rm -i filename
```

- This command will remove the directory dir-name recursively 

```
rm -R dir-name
```

- This command will remove the directory 'dir' recursively, ignoring non-existent files and will never prompt for anything.

```
rm -rf dir_name
```

### rmdir

- This command will remove the directory dir_name, if it's empty. This command can only remove empty directories

```
rmdir dir_name 
```

### mkdir

- This command will create a dir_name

```
mkdir dir_name
```

- This command will create a directory hierarchy. Create parent directories as needed, if they dont exist. You can specify multiple directories.

```
mkdir -p dir_name/dir_name
```

### touch

- This command will create a filename, if it does not exist, otherwise change the timestamp of the file to current time.

```
touch filename
```

### chmod

- This command change the file permissions. Specifications = u user, g group, o other, + add permission, - remove, r read, w write, x execute.

```
chmod <specifications> filename 
```

- This command change the permissions of a directory recursively. To change permission of a directory and everything within that directory, use this command. 

```
chmod -R <specification> dir_name
```

- This command add read permission for the owner and the group.

```
chmod go=+r myfile
```

- This command allow all users to read, write or execute myfile.

```
chmod a +rwx myfile
```

- This command remove read permission from the group and others

```
chmod go -r myfile
```

### chown

- This command change ownership of a file to user 'owner1'.

```
chown owner1 filename
```
### chgrp

- This command change primary group ownership of file 'filename' to group grp_owner.

```
chgrp grp_owner filename
```

- This command change primary group ownership of directory dir_name to group grp_owner recursively. To change group ownership of a directory and everything within that directory, use this command.

```
chgrp -R grp_owner dir_name
```
