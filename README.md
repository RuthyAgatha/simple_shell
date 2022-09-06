# simple_shell
A simple UNIX command interpreter written as part of the ALX C low-level programming project.
Shellby is a simple UNIX command language interpreter that reads commands from either a file or standard input and executes them.
Description
simple_shell is a command line interpreter, or shell, in the tradition of the first Unix shell written by Ken Thompson in 1971. This shell is intentionally minimalistic, yet includes the basic functionality of a traditional Unix-like command line user interface. Standard functions and system calls employed in simple_shell include: access, execve, exit, fork, free, fstat, getline, malloc, perror, signal, stat, wait, write.
File Structure
AUTHORS - List of contributors to this repository
man_1_simple_shell - Manual page for the simple_shell
shell.h - program header file
builtins.c - major builtin functions
check_for_builtins - checks to see if the user's command matches a builtin
new_exit - exits the shell with the option of a specified status
_env - prints the shell's environment variables to the standard output
new_setenv - initializes a new environment variable, or modifies an existing one
new_unsetenv - removes an environment variable
builtins2.c - helper functions for the builtins
add_key - creates a new environment variable
find_key - finds an environment variable in the environment array
add_value - creates a new environment variable string
_atoi - converts a string into a non-negative integer
environment.c - functions related to the environment
make_env - creates the shell's environment from the parent process
free_env - frees the shell's environment
errors.c - functions related to printing errors
print_error - prints an error message to the standard error
_puts2 - prints a string to the standard error
_uitoa - converts an unsigned integer to a string
memory_allocation.c - memory allocation functions
_realloc - a custom realloc function for arrays of pointers
new_strtok.c - custom strtok and helper functions
check_match - checks if a character matches any in a string
new_strtok - a custom strtok for the shell
