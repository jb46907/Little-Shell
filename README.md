# Little Shell (LSH)

**LSH** (Little Shell) is a simple, minimalistic command-line shell written in C. It supports basic built-in commands and allows users to run external system programs by forking child processes.

## Features

- **Built-in Commands:**
  - `cd` — Change the current directory.
  - `help` — Display help text with a list of built-in commands.
  - `exit` — Exit the shell.
  - `echo` — Print text or arguments to the console.
  - `pwd` — Display the current working directory.
  - `whoami` — Print the current user's name.
  - `touch` — Create an empty file.
  - `date` — Display the current system date and time.

- **External Commands:**
  - Run any system command by typing the program name and arguments.
  - The shell uses `fork()` and `execvp()` to execute external programs, allowing users to run commands like `ls`, `grep`, `cat`, etc.

## How to Compile

To compile LSH, simply use `gcc`:

```bash
gcc -o lsh lsh.c
```


This will generate an executable named `lsh`.

## How to Run

Once compiled, run the shell by executing the `lsh` binary:

```bash
./lsh
```

You will be presented with a prompt (`>`), where you can type commands.

## Built-in Commands Usage

Here’s how you can use the built-in commands in LSH:

- **Change Directory (`cd`)**: `cd <directory>`

Example:
```bash
cd /home/user
```

- **Echo Text (`echo`)**: `echo <message>`

Example:
```bash
echo Hello, World!
```

- **Show Current Directory (`pwd`)**:
```bash
pwd
```

- **Display User Name (`whoami`)**:
```bash
whoami
```

- **Create a File (`touch`)**: `touch <filename>`

Example:
```bash
touch myfile.txt
```

- **Display Current Date and Time (`date`)**:
```bash
date
```

- **Exit Shell (`exit`)**:
```bash
exit
```

## External Commands

You can also run any external commands like a regular shell. For example:
```bash
ls -l cat filename.txt
```


## Example Session
```bash
pwd /home/user

whoami user

echo Hello, LSH! Hello, LSH!

touch myfile.txt

ls myfile.txt

date Mon Sep 15 12:34:56 2024

exit
```



## License

This project is open-source under the MIT License. Feel free to use and modify it.

## Contributing

If you want to contribute, feel free to submit a pull request. All contributions are welcome!





