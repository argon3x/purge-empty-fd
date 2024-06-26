# purge-empty-fd (beta)

## Description

`purge-empty-fd` is a script that removes all empty files and directories from a main directory.
this version is still in beta and under testing, but it can be used without any issues. you can also
exclude files and directories to prevent their deletion.

## Usage Mode

* Give execution permissions

```bash
 $ chmod 700 purge-empty-fd
```

* show the help menu

```bash
 $ ./purge-empty-fd -h
```

## Examples

* delete all files from a specific directory

```bash
 $ ./purge-empty-fd -P /directory/path/ -f
```

* delete all directories from a specific directory

```bash
 $ ./purge-empty-fd -P /directory/path/ -d
```

* delete all files and directories in a specified directory

```bash
 $ ./purge-empty-fd -P /directory/path/ -a
```

* exclude files or directories

to exclude multiple files or directories, use the `-E` parameter followed by the
file or directory name, to exclude more that one, separate them with a colon `:`

```bash
 $ ./purge-empty-fd -P /directory/path -a -E file
```

or

```bash
 $ ./purge-empty-fd -P /directory/path -a -E file:directoryL:file2
```

