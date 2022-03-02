##Shell Scripting Basics Exercises

I task that I loved and challenged me well throughout, below are some important commands to know when using Linux

**Task 0**:'pwd' for the print working directory

**Task 1**:'ls' is used to list directory contents

**Task 2**:'cd' is for change directory to home

**Task 3**:'ls -l' list directory contents in long form

**Task 4**: 'ls -al' more detailed list with hidden files and parent directories

**Task 5**: 'ls -al' more detailed list with hidden files and parent directories

**Task 6**: 'mkdir /tmp/my_first_directory' Basic create directory inside the tmp directory

**Task 7**:
  'mv /tmp/betty /tmp/my_first_directory/betty'
  Move file betty, which is located inside the tmp directory, to the tmp directory created earlier.
  This exercise required some dir traversing.

**Task 8**:
  'rm /tmp/my_first_directory/betty'
  Remove file betty located in tmp/my_first_directory directory created earlier.

**Task 9**:
  'rmdir /tmp/my_first_directory'
  Standard directory deletion.

**Task 10**:
  'cd -'
  Changes to previous directory you were in.

**Task 11**:
  'ls -la . .. /boot'
  List all files/directories, including hidden files/directories, from 3 separate directories: current directory, parent of working directory, and /boot directory.
  The ls command allows multiple directories to be listed separated by spaces.

**Task 12**:
  'file /tmp/iamafile'
  Prints the type of file iamafile.

**Task 13**:
  'ln -s /bin/ls __ls__'
  Create a symbolic link named __ls__ for /bin/ls

Exercise 14:
  cp -u *.html ..
  Copy all html files from the current directory to the parent directory, but only copy files that didn't exist in the parent directory or are newer versions than the ones that already exist in the parent directory.
  The -u option didn't show on the terminal manual page. The -u option copies the file into the directory if its a newer version. If the file doesn't exist in the directory, it will copy over.
  The -n option works for copying files that don't exist in the parent directory, but it doesn't check if the file is a newer version or not.

Exercise 15:
  mv [[:upper:]]* /tmp/u
  Move all files that begin with a capital letter to /tmp/u

Exercise 16:
  rm *~
  Deletes all files in the current directory that end with a ~

Exercise 17:
  mkdir -p welcome/to/holberton
  Create directory `welcome` in current directory. Create directory `to` inside directory `welcome`. Create directory `holberton` inside directory `to`.
  The -p option creates any intermediate directories in the path argument.

Exercise 18:
  ls -pam
  List all files and directories of the current directory, separated by commas. Directory names should end with a `/`. The listing should be alph ordered, except for dot (.) or dot dot (..), which should be listed at the beginning.
  The -a option is to show any hidden files.
  The -p option writes a `/` at the end of directory names.
  The -m option streams the output, separating each listing with commas.

Exercise 19:
  0 string HOLBERTON Holberton data
  !:mime Holberton
  Create a magic file called `holberton.mgc` that can be used with the command `file` to detect `Holberton` data files. Holberton data files always contain "HOLBERTON" at offset 0.

  This exercise was much different from the previous exercises. From what I understand, the magic file is used to detect patterns in files and will give a specified output depending on a matching pattern.
  The first argument is a number representing the offset.
  The second argument is the data type you are searching for. In our case, it is a string.
  The third argument is the data you are searching for. In our case, "HOLBERTON", which we specified as a string in the second argument.
  The fourth argument is the message you want to output on match. If the search matches, it will output this message.
  The last argument is separated by a line. Since the fourth argument can be long and contain multiple strings, we separate the fourth and fifth arguments with this new line. This last argument can be multiple different things. In this case, a MIME type.
  According to bash manual, a "MIME type is given on a separate line, which must be the next non-blank or comment line after the magic line that identifies the file type".
  I knew to search for a MIME type because the example provided:
  $ file --mime-type -m holberton.mgc *
  The above returns message "Holberton" when matching a MIME ?? Not exactly sure, but this is what I can tell from what I've tested out and can see from the output and examples.
  $ file -m holberton.mgc *
  The above will return message "Holberton data" for any offset 0 "HOLBERTON" matches.
  A cool thing to note is that the `file` command is compiling and running the magic file. So there is no need to compile to magic "permanently".
  NOTE: Compiling a magic source file:
  $ file -C -m <filename>.mgc
  This produces the compiled magic file.
  $ file -i -m <filename>.mgc *
  This allows you to use the compiled file by specifying its name using the -m switch again.
