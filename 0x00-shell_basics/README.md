##Shell Scripting Basics Exercises

I task that I loved and challenged me well throughout, below are some important commands to know when using Linux.

**Task 0:** 'pwd' for the print working directory

**Task 1:** 'ls' is used to list directory contents

**Task 2:** 'cd' is for change directory to home

**Task 3:** 'ls -l' list directory contents in long form

**Task 4:** 'ls -al' more detailed list with hidden files and parent directories

**Task 5:** 'ls -al' more detailed list with hidden files and parent directories

**Task 6:** 'mkdir /tmp/my_first_directory' Basic create directory inside the tmp directory

**Task 7:**
  'mv /tmp/betty /tmp/my_first_directory/betty'
  Move file betty, which is located inside the tmp directory, to the tmp directory created earlier.
  This exercise required some dir traversing.

**Task 8:**
  'rm /tmp/my_first_directory/betty'
  Remove file betty located in tmp/my_first_directory directory created earlier.

**Task 9:**
  'rmdir /tmp/my_first_directory'
  Standard directory deletion.

**Task 10:**
  'cd -'
  Changes to previous directory you were in.

**Task 11:**
  'ls -la . .. /boot'
  List all files/directories, including hidden files/directories, from 3 separate directories: current directory, parent of working directory, and /boot directory.
  The ls command allows multiple directories to be listed separated by spaces.

**Task 12:**
  'file /tmp/iamafile'
  Prints the type of file iamafile.

**Task 13:**
  'ln -s /bin/ls __ls__'
  Create a symbolic link named __ls__ for /bin/ls

**Task 14:**
  'cp -u *.html ..'
  Copy all html files from the current directory to the parent directory, but only copy files that didn't exist in the parent directory or are newer versions than the ones that already exist in the parent directory.

**Task 15:**
  'mv [[:upper:]]* /tmp/u'
  Move all files that begin with a capital letter to /tmp/u

**Task 16:**
  'rm *~'
  Deletes all files in the current directory that end with a ~

**Task 17:**
  'mkdir -p welcome/to/school'
  The -p option creates any intermediate directories in the path argument.

**Task 18:**
  'ls -al -m --indicator-style=slash -v -c'
  The -al was for List all files and directories of the current directory
  The -m was to separated by commas.
  THe --indicator-style=slash was to show Directory names  with a `/`.
  The -v was The listing should be alph ordered, except for dot (.) or dot dot (..), which should be listed at the beginning.
  The -c option is to show any hidden the numbers in order

**Task 19:**
  0   string  SCHOOL School data
  !:mime  School

  Create a file called `school` that can be used with the command `file` to detect `School` data files. School data files that contain "SCHOOL" at offset 0.
