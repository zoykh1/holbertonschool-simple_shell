<img align="center" width="35%" src="https://cdn.prod.website-files.com/64107f65f30b69371e3d6bfa/65c6179aa44b63fa4f31e7ad_Holberton-Logo-Cherry.svg">

# Simple Shell Project

## Table of Contents

<img align="right" width="35%" src="https://cdn-icons-png.flaticon.com/512/1672/1672361.png">

- [Description](#description)
- [Function Prototype](#function-prototype)
- [Features](#features)
- [Compilation](#compilation)
- [Requirements](#requirements)
- [Examples](#examples)
- [Man Page](#man-page)
- [Flowchart](#flowchart)
- [Tests and Valgrind](#tests-and-valgrind)
- [Authors](#authors)
- [Notes](#notes)

## Description
This project is a simple command-line interpreter (shell) implemented in C. It replicates certain functionalities of `/bin/sh` and can operate in both interactive and non-interactive modes.

## Function Prototype
```c
int main(int argc, char **argv);
```

## Features
```markdown
- Execution of basic shell commands.
- Error handling with custom error messages.
- Process management using `fork`, `execve`, and `wait`.
- Utilization of the `PATH` environment variable to locate binaries.
- Signal handling and EOF (`Ctrl+D`) management.
```

## Compilation
To compile the project, use the following command:
```bash
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```

## Requirements
```markdown
- Ubuntu 20.04 LTS
- GCC
- Git
```

## Examples

### Interactive Mode
```bash
$ ./hsh
($) ls
main.c shell.c hsh
($) pwd
/home/user/simple_shell
($) exit
```

### Non-Interactive Mode
```bash
$ echo "ls -l" | ./hsh
-rw-r--r-- 1 user user 1234 Jan 9 10:00 main.c
-rw-r--r-- 1 user user 5678 Jan 9 10:01 shell.c
$ echo "pwd" | ./hsh
/home/user/simple_shell
```

## Man Page
The command to display the man page is:
```bash
man ./man_1_simple_shell.1
```

Example of the man page content:
```plaintext
.TH SIMPLE_SHELL 1 "January 2025" "Version 1.0" "User Manual"

.SH NAME
simple_shell \- custom command-line interpreter

.SH SYNOPSIS
.B ./hsh
```

## Flowchart
```markdown
![Flowchart](https://cdn-icons-png.flaticon.com/512/2545/2545814.png)
```

## Tests and Valgrind
To test for memory management:
```bash
valgrind --leak-check=full ./hsh
```

## Authors
```markdown
- [@Zoy](https://github.com/zoykh1)
```

## Notes
```markdown
- This project follows the Betty coding style.
- No memory leaks are tolerated.
```
